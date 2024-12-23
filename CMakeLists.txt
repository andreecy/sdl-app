cmake_minimum_required(VERSION 3.10)
project(SdlApp VERSION 1.0)

set(CMAKE_CXX_FLAGS "-std=c++17 -Wall -Wextra")

add_executable(sdlapp main.cpp)

add_subdirectory(vendor/SDL2)
target_link_libraries(sdlapp SDL2)
