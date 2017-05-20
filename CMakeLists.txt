cmake_minimum_required(VERSION 3.4.1)

include_directories( . include ../libogg/include ../opus/include )

add_definitions(-DOP_FIXED_POINT)

add_library( opusfile STATIC
src/http.c
src/info.c
src/internal.c
src/opusfile.c
src/stream.c
src/wincerts.c )

