cmake_minimum_required(VERSION 3.22)

if(NOT DEFINED ${CMAKE_CUDA_ARCHITECTURES})
    set(CMAKE_CUDA_ARCHITECTURES 52 61 75)
endif()

project(nbody_cuda CUDA CXX)

set(CMAKE_CXX_STANDARD 17)

find_package(CUDA REQUIRED)

add_subdirectory(external/grassland)
add_subdirectory(shaders)
add_subdirectory(src)
