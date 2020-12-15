cmake_minimum_required(VERSION 3.15.0-rc1)

set(CMAKE_GENERATOR_PLATFORM x64)

project(vul2_engine)

# creating the library
add_library(${PROJECT_NAME} src/Vulture.cpp src/Vulture.hpp)

set(LIBRARY_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin/${CMAKE_BUILD_TYPE})
