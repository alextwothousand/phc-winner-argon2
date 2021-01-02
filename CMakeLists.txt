cmake_minimum_required(VERSION 3.17)
project(Argon2)

file(GLOB_RECURSE src_sources src/*.c)
file(GLOB_RECURSE src_headers src/*.h)

add_library(Argon2 STATIC include/argon2.h ${src_sources} ${src_headers})
target_include_directories(Argon2 PRIVATE include/)