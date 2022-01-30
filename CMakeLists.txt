cmake_minimum_required(VERSION 3.0)

project(usermem)

add_library(usermem source/user_mem.c source/user_new.cpp)
target_include_directories(usermem PRIVATE include)
target_link_libraries(usermem SceLibcInternal c)
