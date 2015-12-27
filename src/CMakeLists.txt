cmake_minimum_required(VERSION 2.6)

project(libcanard-demo)

set(CMAKE_BUILD_TYPE Debug)

find_package(Threads)

file(GLOB src *.c)

add_executable(
    node-demo
    ${src}
)

target_link_libraries (node-demo ${CMAKE_THREAD_LIBS_INIT})
