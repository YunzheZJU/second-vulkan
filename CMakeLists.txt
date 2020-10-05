cmake_minimum_required(VERSION 3.17)
project(second_vulkan)

set(CMAKE_CXX_STANDARD 17)

set(SOURCE_FILES main.cpp)

include_directories(include)

link_directories(lib)

add_executable(second_vulkan ${SOURCE_FILES})

target_link_libraries(second_vulkan vulkan-1.lib glfw3.lib)