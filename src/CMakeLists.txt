file(GLOB source_files *.cpp *.h *.cu *.cuh)

add_executable(nbody)

target_link_libraries(nbody PRIVATE grassland)
target_include_directories(nbody PRIVATE ${GRASSLAND_INCLUDE_DIRS} ${CMAKE_CUDA_TOOLKIT_INCLUDE_DIRECTORIES})
target_sources(nbody PRIVATE ${source_files})
add_dependencies(nbody compiled_shaders_target)
