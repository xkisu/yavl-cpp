cmake_minimum_required(VERSION 3.12)
project(yavl-cpp)

set(CMAKE_CXX_STANDARD 14)

set(YAML-CPP_INCLUDE_DIR "../yaml-cpp/include" CACHE PATH "Path to the yaml-cpp include directories")

message(STATUS "yavl-cpp using yaml-cpp in directory ${YAML-CPP_INCLUDE_DIR}")

include_directories(src)
include_directories(${YAML-CPP_INCLUDE_DIR})

add_library(yavl-cpp STATIC
        src/yavl.cpp
        src/yavl.h
        )