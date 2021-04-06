# CMAKE Version
cmake_minimum_required(VERSION 3.10)

# CXX STDANDARD
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Project Name
project(my_project)

# Binary Directories
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR}/out/bin)

# Library Directories
set(LIBRARY_OUTPUT_PATH ${CMAKE_CURRENT_SOURCE_DIR}/out/lib)

# Link Directories
LINK_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/out/lib)

# Include Directories
INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/include)

# Submodule
ADD_SUBDIRECTORY(${CMAKE_CURRENT_SOURCE_DIR}/src)
