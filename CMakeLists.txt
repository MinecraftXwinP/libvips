cmake_minimum_required(VERSION 3.2)

include(cmake/HunterGate.cmake)

HunterGate(
    URL "https://github.com/ruslo/hunter/archive/v0.23.57.tar.gz"
    SHA1 "8befbbaea51cb54681f6e690212ed753ae807529"
)

project(vips) 

add_subdirectory(libvips)

