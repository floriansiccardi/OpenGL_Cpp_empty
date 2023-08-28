# from path/CMakeLists.txt

cmake_minimum_required(VERSION 3.10)
project(DoublePendulum)

# Settings
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/Bin)

link_directories(${CMAKE_SOURCE_DIR}/Lib)
include_directories(${CMAKE_SOURCE_DIR}/ThirdParty)

# Subdirectories
add_subdirectory(Main/Source)