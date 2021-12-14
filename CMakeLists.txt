cmake_minimum_required(VERSION 3.22)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CXX_FLAGS_WARNINGS "-O3 -Wall -Wextra -Wpedantic -Wshadow")
set(CMAKE_CXX_FLAGS ${CXX_FLAGS_WARNINGS})

project(<ProjectName> VERSION 1.0 LANGUAGES CXX)

set(PROJECT_INCLUDE_DIRS include/)
include_directories(${PROJECT_INCLUDE_DIRS})
set(PROJECT_SOURCE_FILES src/example.cpp)
set(PROJECT_OUTPUT_NAME ProjectName_Executable)

add_executable(${PROJECT_OUTPUT_NAME} ${PROJECT_SOURCE_FILES})

