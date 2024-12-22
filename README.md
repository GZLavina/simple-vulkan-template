# Vulkan Starter Project

This is a simple template project to get a Vulkan development environment setup with CMake and vcpkg.

Vulkan and vcpkg have to be manually downloaded and their environment variables correctly set.

The "default" CMake preset uses the standard vcpkg toolchain with MSBuild.

## How to use

On Windows, with Vulkan and vcpkg correctly installed:

1. Clone the repository.
2. Navigate to the repository root.
3. Run `cmake --preset default` and then `cmake --build build --preset default`. This step takes a while.
4. You should see a new window with a white background, as shown in the "Development Environment" section of Vulkan Tutorial.

**Other platforms will require new presets in `CMakePresets.json`.**

This sequence of steps is IDE agnostic, but you can easily configure VS, VSCode or CLion to use the "default" preset and configure, build and run with the click of a button.