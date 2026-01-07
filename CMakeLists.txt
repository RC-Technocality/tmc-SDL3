cmake_minimum_required(VERSION 3.16)
project(tmc-sdl3)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

# This assumes the SDL source is available in vendored/SDL
add_subdirectory(vendored/SDL EXCLUDE_FROM_ALL)

# Create your game executable target as usual
add_executable(tmc-sdl3 root_main.c)

# Link to the actual SDL3 library.
target_link_libraries(tmc-sdl3 PRIVATE SDL3::SDL3)

# Platform definitions
if (WIN32)
    target_compile_definitions(tmc-sdl3 PRIVATE PLATFORM_WINDOWS)
elseif (UNIX)
    target_compile_definitions(tmc-sdl3 PRIVATE PLATFORM_LINUX)
endif()

# Warnings
if (MSVC)
    target_compile_options(tmc-sdl3 PRIVATE /W4 /permissive-)
else()
    target_compile_options(tmc-sdl3 PRIVATE -Wall -Wextra -Wpedantic)
endif()