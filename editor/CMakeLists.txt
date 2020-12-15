cmake_minimum_required(VERSION 3.15.0-rc1)

set(CMAKE_GENERATOR_PLATFORM x64)

project(vul2_editor)
add_executable(${PROJECT_NAME} src/main.cpp)

#include engine
target_include_directories(${PROJECT_NAME} PUBLIC ../engine/include PRIVATE ../engine/src)
target_link_libraries(${PROJECT_NAME} PRIVATE vul2_engine)

set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin/${CMAKE_BUILD_TYPE})