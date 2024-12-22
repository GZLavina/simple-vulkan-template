cmake_minimum_required(VERSION 3.27)
project(VulkanBase CXX)

find_package(Vulkan REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
find_package(Stb REQUIRED)
find_package(glm CONFIG REQUIRED)
find_package(assimp CONFIG REQUIRED)

set(CMAKE_CXX_STANDARD 20)

add_executable(VulkanBase main.cpp)

target_include_directories(
        VulkanBase PRIVATE ${Stb_INCLUDE_DIR}
)

target_link_libraries(VulkanBase PRIVATE
        Vulkan::Vulkan
        glfw
        glm::glm
        assimp::assimp
)
