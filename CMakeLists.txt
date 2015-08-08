# Created by Hal@shurabaP
# This code is under The BSD 3-Clause License.
# See more Licence.txt.
cmake_minimum_required(VERSION 3.2)
project(world)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES main/cheaptrick.cpp main/cheaptrick.h main/common.cpp main/common.h main/constantnumbers.h main/d4c.cpp main/d4c.h main/dio.cpp main/dio.h main/fft.cpp main/fft.h main/matlabfunctions.cpp main/matlabfunctions.h main/stonemask.cpp main/stonemask.h main/synthesis.cpp main/synthesis.h)

add_library(world ${SOURCE_FILES})

target_include_directories(world PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
