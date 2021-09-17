cmake_minimum_required(VERSION 3.20)
project(lbireVoxel)

set(CMAKE_CXX_STANDARD 20)
cmake_minimum_required(VERSION 3.7)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

add_executable(lbireVoxel src/main.cpp)
target_link_libraries(lbireVoxel ${SDL2_LIBRARIES})
