cmake_minimum_required(VERSION 3.12)
project(yavl-cpp)

set(CMAKE_CXX_STANDARD 14)
set(YAML-CPP_INCLUDE_DIR "../yaml-cpp" CACHE PATH "Path to yaml-cpp")

include_directories(src)
include_directories(${YAML-CPP_INCLUDE_DIR})

add_library(yavl-cpp STATIC
    src/yavl.cpp
    src/yavl.h
)