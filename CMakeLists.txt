cmake_minimum_required(VERSION 3.10)

project(test)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

file(GLOB_RECURSE CXX_SOURCES "src/*.cc")
add_executable(${PROJECT_NAME} ${CXX_SOURCES})
target_include_directories(${PROJECT_NAME} PRIVATE include)