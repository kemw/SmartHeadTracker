PROJECT( SmartHeadTracker_project )
FIND_PACKAGE( OpenCV 3.0 REQUIRED HINTS /usr/local/Cellar/opencv3/3.1.0_1)
cmake_minimum_required(VERSION 2.8)

SET(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR}/bin)
set(CMAKE_BINARY_DIR ${PROJECT_BINARY_DIR}/bin)

set(PS3_INCLUDE ${CMAKE_SOURCE_DIR}/PS3EYEDriver/src)
file(GLOB PS3_SOURCES "${CMAKE_SOURCE_DIR}/PS3EYEDriver/src/*.cpp")

add_subdirectory(src)
