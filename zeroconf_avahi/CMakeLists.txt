##############################################################################
# CMake
##############################################################################

cmake_minimum_required(VERSION 2.4.6)
include($ENV{ROS_ROOT}/core/rosbuild/rosbuild.cmake)

set(CMAKE_VERBOSE_MAKEFILE TRUE)

##############################################################################
# Ros
##############################################################################

rosbuild_init()

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

##############################################################################
# Project
##############################################################################

add_subdirectory(src)