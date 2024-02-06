cmake_minimum_required(VERSION 3.1.0)
project (test_dll_gen C)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "../../output")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "../../output")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "../../output")

INCLUDE_DIRECTORIES("./")

add_library(test_dll_gen SHARED my_lib.c)

