cmake_minimum_required(VERSION 3.3)
project(voro2b)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Wall -ansi -pedantic -O3 -lvoro++")

include_directories(/usr/local/include/voro++)
link_directories(/usr/local/lib)



set(SOURCE_FILES main.cpp CSCalculation.h CSCalculation.cpp CSSolver.cpp CSSolver.h)
add_executable(voro2b ${SOURCE_FILES})
