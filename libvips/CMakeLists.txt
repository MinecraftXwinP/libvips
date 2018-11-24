hunter_add_package(glib)
find_package(glib-2.0 CONFIG REQUIRED)
set(VIPS_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include)
add_subdirectory(histogram)
# add_subdirectory(convolution)
add_subdirectory(foreign)
add_subdirectory(colour)
# add_subdirectory(freqfilt)
# add_subdirectory(iofuncs)
# add_subdirectory(morphology)
# add_subdirectory(draw)
# add_subdirectory(create)
# add_subdirectory(resample)
# add_subdirectory(mosaicing)
# add_subdirectory(arithmetic)
add_subdirectory(conversion)
add_library(vips IMPORTED)
target_include_directories(vips PRIVATE ${GLIB2_INCLUDE_DIRS})
target_link_libraries(
    vips
    colour
    conversion
    foreign
    histogram
)
