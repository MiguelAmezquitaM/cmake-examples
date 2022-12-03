cmake_minimum_required(VERSION 3.0)

project(example)

add_subdirectory(libs)

add_executable(example
    src/main.cpp
    libs
)

target_link_libraries(example PRIVATE liba)
target_link_libraries(example PRIVATE libb)

set(CMAKE_CXX_FLAGS "-std=c++17")
set(CMAKE_EXE_LINKER_FLAGS "-static")