SET(LIBTGA_SRCS
    tga.c
    tgaconfig.h
    tga.h
    tgaread.c
    tgawrite.c )

ADD_LIBRARY(tga STATIC
            ${LIBTGA_SRCS} )

TARGET_INCLUDE_DIRECTORIES(tga PUBLIC
    "${CMAKE_CURRENT_SOURCE_DIR}" )
                           
