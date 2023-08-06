cmake_minimum_required(VERSION 3.0)
project( DORO_01 )

set(CMAKE_POSITION_INDEPENDENT_CODE ON)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fpermissive")

# SOURCES
file( GLOB_RECURSE MY_SRC ./src/*.cc )

add_executable( doro_0x01 ${MY_SRC} ${MY_SRC} )
target_link_libraries( doro_0x01 pthread rtaudio )
