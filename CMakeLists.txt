cmake_minimum_required(VERSION 3.20)

project(DragonPhysics VERSION ${DragonEngine_VERSION})

if(NOT TARGET Dragon::Core)
    find_package(DragonCore REQUIRED)
endif()

if(NOT TARGET Dragon::Compute)
    find_package(DragonCompute REQUIRED)
endif()

add_subdirectory(src)