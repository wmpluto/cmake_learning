cmake_minimum_required(VERSION 3.1.0)
project (device_update C)

set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "../../output")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "../../output")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "../../output")

INCLUDE_DIRECTORIES("../dll_gen")
INCLUDE_DIRECTORIES("./")

link_directories("../output")

add_executable(demo main.c)
target_link_libraries(demo test_dll_gen)
