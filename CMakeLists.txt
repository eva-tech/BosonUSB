cmake_minimum_required(VERSION 3.10)
project( BosonUSB )
include_directories(${PROJECT_SOURCE_DIR})
find_package( OpenCV REQUIRED )
add_executable( BosonUSB BosonUSB.cpp )
target_link_libraries( BosonUSB ${OpenCV_LIBS} )

install (TARGETS BosonUSB RUNTIME DESTINATION bin)