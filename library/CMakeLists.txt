cmake_minimum_required(VERSION 3.4)

project(mylibrary)

if("${CMAKE_SOURCE_DIR}" STREQUAL "${CMAKE_BINARY_DIR}")
    message(FATAL_ERROR "Please create a subfolder and build inside there. ")
endif()

# compile library as shared 
add_library("${CMAKE_PROJECT_NAME}" SHARED ./mylibrary.cpp)

# remove the library PREFIX to an empty string.
set_target_properties("${CMAKE_PROJECT_NAME}" PROPERTIES PREFIX "")