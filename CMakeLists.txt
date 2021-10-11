cmake_minimum_required(VERSION 3.0)

project(meta2alt)

add_executable(meta2alt meta2alt.c)
target_compile_options(meta2alt PRIVATE -Wall -Wextra)

install(TARGETS meta2alt RUNTIME DESTINATION bin)
