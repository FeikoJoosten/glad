cmake_minimum_required(VERSION 3.0)
project(glad)

file(GLOB_RECURSE GLAD_SOURCES "include/*.h" "src/*.c")

add_library(glad STATIC ${GLAD_SOURCES})
target_include_directories(glad PUBLIC include/)