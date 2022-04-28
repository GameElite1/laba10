cmake_minimum_required(VERSION 3.1)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(vosved_v_kvadrat)

add_executable(prog ./prog/prog.cpp)

include_directories(./bibl)
add_subdirectory(./kvadrat kvadrat)

target_link_libraries(prog kvadrat)