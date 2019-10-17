# CMakeList.txt : CMake project for CMakeProject1, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.5)

set(CMAKE_CXX_STANDARD 11)

project(onefile)
# Add source to this project's executable.
add_executable (onefile main.cpp)
