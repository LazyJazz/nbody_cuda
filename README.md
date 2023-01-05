# nbody_cuda

## Build Guide

This repo uses Grassland - a graphics library based on Vulkan.
It is integrated as an submodule. Which means, you need to clone this repo with `--recursive` option.

```shell
git clone https://github.com/LazyJazz/nbody_cuda.git --recursive
```

or, you can use the following command to pull submodules in a existed local repo:

```shell
git submodule update --init --recursive
```

### Requirements

CUDA Toolkit: [Download Page](https://developer.nvidia.com/cuda-downloads)

Vulakn SDK: [Download Page](https://vulkan.lunarg.com/sdk/home)

CMake: [Official Site](https://cmake.org/)

### Build This Project

```shell
mkdir build
cd build
cmake ..
cmake --build .
```

### Run

```shell
# Move current working path to build/src directory
./nbody     # Unix-Like OS
.\nbody.exe # Windows
```
