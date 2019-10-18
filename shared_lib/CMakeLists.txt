# CMakeList.txt : CMake project for CMakeProject1, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.5)

set(CMAKE_CXX_STANDARD 11)

project(link_lib)

set(MATHLIB_SRC MathFuncs.cpp MathFuncs.h)
add_library(mathlib STATIC ${MATHLIB_SRC})

add_executable(link_lib main.cpp)
target_link_libraries(link_lib mathlib)