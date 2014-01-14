cmake_minimum_required (VERSION 2.8) 
project(hybris-cam-demo) 

add_executable (hybris-cam-demo direct_camera_test.cpp)

target_link_libraries (hybris-common hybris-cam-demo) 