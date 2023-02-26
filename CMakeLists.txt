cmake_minimum_required(VERSION 3.16)
project(sophist VERSION 0.0.0 LANGUAGES C)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_library(sophist
    src/sophist.c
    include/sophist.h
)
target_include_directories(sophist PUBLIC include)

add_subdirectory(tools/cli EXCLUDE_FROM_ALL)
