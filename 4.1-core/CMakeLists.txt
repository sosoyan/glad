cmake_minimum_required(VERSION 3.5)
project(glad LANGUAGES C)

include_directories(include)
add_library(glad STATIC src/glad.c)
set_target_properties(glad PROPERTIES LINKER_LANGUAGE C)
set_target_properties(glad PROPERTIES COMPILE_FLAGS "-fPIC")