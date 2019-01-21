cmake_minimum_required(VERSION 3.13)
project(recastCLI_js)

set(CMAKE_CXX_STANDARD 14)
SET(CMAKE_EXE_LINKER_FLAGS "-static")

include_directories(main)
include_directories(recast)

add_executable(recastCLI_js
        main/build.cpp
        main/build.h
        main/ChunkyTriMesh.cpp
        main/ChunkyTriMesh.h
        main/InputGeom.cpp
        main/InputGeom.h
        main/main.cpp
        main/MeshLoaderObj.cpp
        main/MeshLoaderObj.h
        recast/Recast.cpp
        recast/Recast.h
        recast/RecastAlloc.cpp
        recast/RecastAlloc.h
        recast/RecastArea.cpp
        recast/RecastAssert.cpp
        recast/RecastAssert.h
        recast/RecastContour.cpp
        recast/RecastFilter.cpp
        recast/RecastLayers.cpp
        recast/RecastMesh.cpp
        recast/RecastMeshDetail.cpp
        recast/RecastRasterization.cpp
        recast/RecastRegion.cpp)
