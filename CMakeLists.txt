
cmake_minimum_required(VERSION 3.10)

set(project_name add)
project(${project_name})
include_directories("${CMAKE_SOURCE_DIR}")


add_library(add_lib "add.h" "add.cpp")
add_executable(add_exe "main.cpp")
target_link_libraries(add_exe add_lib)
message(STATUS "Done")