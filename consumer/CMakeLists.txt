cmake_minimum_required(VERSION 3.4)

project("consumer")

set(CMAKE_CXX_STANDARD 14)

# write program to bin folder 
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

include_directories("${CMAKE_SOURCE_DIR}/../library/")

add_executable("${CMAKE_PROJECT_NAME}" main.cpp)

target_link_libraries("${CMAKE_PROJECT_NAME}" "${CMAKE_SOURCE_DIR}/../library/build/mylibrary.dylib")


