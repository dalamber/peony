cmake_minimum_required(VERSION 3.5)
project(peony)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/out)

add_subdirectory(peony-common)
add_subdirectory(peony-client)
add_subdirectory(peony-svc)
add_subdirectory(peony-tester)