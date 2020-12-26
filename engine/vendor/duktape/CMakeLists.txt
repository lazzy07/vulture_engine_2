cmake_minimum_required(VERSION 3.15.0-rc1)
set(CMAKE_GENERATOR_PLATFORM x64)

project(vul_js_scriptor)

add_library(${PROJECT_NAME} src/duk_config.h src/duktape.h src/duktape.c)

set(LIBRARY_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin/${CMAKE_BUILD_TYPE})