cmake_minimum_required(VERSION 3.0)

project(liba)


include_directories(include)

add_library(
    liba
    "${CMAKE_CURRENT_SOURCE_DIR}/src/liba.cpp"
)

target_include_directories(liba PUBLIC include)