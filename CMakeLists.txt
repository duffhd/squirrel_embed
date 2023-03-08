cmake_minimum_required(VERSION 3.24)
project(squirrel_embed)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(libs)

add_executable(squirrel_embed src/main.cpp)

target_include_directories(squirrel_embed PUBLIC libs/squirrel/include)
target_link_libraries(squirrel_embed squirrel sqstdlib)
