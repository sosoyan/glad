cmake_minimum_required(VERSION 3.5)
project(glad410 LANGUAGES C)

include_directories(include)
add_library(glad410 STATIC src/glad.c)
set_target_properties(glad410 PROPERTIES LINKER_LANGUAGE C)
set_target_properties(glad410 PROPERTIES COMPILE_FLAGS "-fPIC")
