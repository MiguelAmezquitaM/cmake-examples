cmake_minimum_required(VERSION 3.0)

project(libb)

add_library(
    libb
    "${CMAKE_CURRENT_SOURCE_DIR}/src/libb.cpp"
)

include_directories(include)

target_include_directories(libb PUBLIC include)
