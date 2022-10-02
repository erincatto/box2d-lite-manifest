cmake_minimum_required(VERSION 3.24)

message(STATUS "cmake tool chain: ${CMAKE_TOOLCHAIN_FILE}")

project(box2d-lite LANGUAGES CXX)

add_subdirectory(src)
add_subdirectory(samples)
