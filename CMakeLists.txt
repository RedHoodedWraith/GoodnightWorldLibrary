cmake_minimum_required(VERSION 3.16)
project(GoodnightWorldLibrary VERSION 1.0)

set(CMAKE_CXX_STANDARD 11)

add_library(GoodnightWorldLibrary goodnight.cpp goodnight.h)

install(TARGETS GoodnightWorldLibrary DESTINATION lib)
install(FILES goodnight.h DESTINATION include)
