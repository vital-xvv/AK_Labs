cmake_minimum_required(VERSION 3.5 FATAL_ERROR)

project(hw)

add_executable(hello main.cpp)

add_library(message STATIC message.h message.cpp)

target_link_libraries(hello message)
