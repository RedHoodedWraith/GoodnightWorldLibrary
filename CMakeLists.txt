cmake_minimum_required(VERSION 3.16)
project(GoodnightWorldLibrary VERSION 1.0)

set(CMAKE_CXX_STANDARD 11)

include_directories(lib)
add_subdirectory(lib)

install(FILES goodnight.h goodnight.cpp DESTINATION include)

add_executable(Demo main.cpp)
target_link_libraries(Demo ${CMAKE_PROJECT_NAME})