cmake_minimum_required(VERSION 3.17)
project(second_vulkan)

set(CMAKE_CXX_STANDARD 17)

set(SOURCE_FILES main.cpp)

# Choose the glfw lib according to your compiler
# MSVC
set(GLFW_LIBRARY glfw3.lib)
# MinGW-W64
#set(GLFW_LIBRARY libglfw3.a)

set(LIBRARIES vulkan-1.lib ${GLFW_LIBRARY})

include_directories(include)

link_directories(lib)

add_executable(second_vulkan ${SOURCE_FILES})

target_link_libraries(second_vulkan ${LIBRARIES})