cmake_minimum_required(VERSION 3.5)
project(glad430 LANGUAGES C)

include_directories(include)
add_library(glad430 STATIC src/glad.c)
set_target_properties(glad430 PROPERTIES LINKER_LANGUAGE C)
set_target_properties(glad430 PROPERTIES COMPILE_FLAGS "-fPIC")
