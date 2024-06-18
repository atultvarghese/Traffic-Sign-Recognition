cmake_minimum_required(VERSION 3.20)
project(object_detection_v8)


find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable( object_detection_v8 main.cpp )
target_link_libraries( object_detection_v8 ${OpenCV_LIBS} )