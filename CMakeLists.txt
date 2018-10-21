cmake_minimum_required(VERSION 3.12)
project(yavl-cpp)

set(CMAKE_CXX_STANDARD 14)

include_directories(src)

add_library(yavl-cpp STATIC
    src/yavl.cpp
    src/yavl.h
)