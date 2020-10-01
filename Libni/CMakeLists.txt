cmake_minimum_required(VERSION 3.17)
project(Libni)

set(CMAKE_CXX_STANDARD 20)

add_library(Libni src/library.cpp headers/library.h)