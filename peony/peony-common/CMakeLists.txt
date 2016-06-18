cmake_minimum_required(VERSION 3.5)
project(peony-common)

set(LIB_NAME "peony-common")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/out)

file(GLOB_RECURSE SOURCE_FILES
        src/*.h
        src/*.cpp)

add_library(${LIB_NAME} STATIC ${SOURCE_FILES})