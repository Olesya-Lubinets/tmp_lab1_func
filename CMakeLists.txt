cmake_minimum_required(VERSION 3.14)
project(Lab1)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD 11 )
set(CMAKE_CXX_FLAGS_RELEAse "/MT")
set(CMAKE_CXX_FLAGS_DEBUG "/MTd")
add_subdirectory(lib/googletest-master)
enable_testing()
include_directories(lib/googletest-master/googletest/include)
add_executable(Lab1 main.cpp text.cpp text.h tests_1/Unit_test.cpp)
target_link_libraries(Lab1 gtest)

