add_library(
    colour
    Lab2LabS.c
    Lab2LabQ.c
    LabQ2LabS.c
    dECMC.c
    LabQ2sRGB.c
    Lab2LCh.c
    XYZ2scRGB.c
    scRGB2sRGB.c
    colour.c
    pcolour.h
    scRGB2XYZ.c
    UCS2LCh.c
    LCh2UCS.c
    icc_transform.c
    dE00.c
    Lab2XYZ.c
    XYZ2Yxy.c
    sRGB2HSV.c
    float2rad.c
    XYZ2Lab.c
    HSV2sRGB.c
    dE76.c
    sRGB2scRGB.c
    Yxy2XYZ.c
    LabS2Lab.c
    scRGB2BW.c
    colourspace.c
    LabQ2Lab.c
    LabS2LabQ.c
    LCh2Lab.c
    rad2float.c
)

target_include_directories(colour PUBLIC ${VIPS_INCLUDE_DIR})

target_link_libraries(colour PkgConfig::glib-2.0)
