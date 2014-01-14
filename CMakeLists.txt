cmake_minimum_required (VERSION 2.8) 
project(hybris-cam-demo) 


include_directories(${CMAKE_CURRENT_SOURCE_DIR})
add_executable (hybris-cam-demo direct_camera_test.cpp)
add_library(camera SHARED IMPORTED )

target_link_libraries (hybris-cam-demo camera) 