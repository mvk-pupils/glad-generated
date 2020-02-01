cmake_minimum_required(VERSION 3.0)
project(Glad)

add_library(glad include/glad/glad.h src/glad.c)
target_include_directories(glad PUBLIC include/)

set(GLAD_INCLUDE_DIRS "${CMAKE_CURRENT_BINARY_DIR}/include/" PARENT_SCOPE)
set(GLAD_LIBRARIES glad PARENT_SCOPE)
