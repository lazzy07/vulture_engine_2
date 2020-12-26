cmake_minimum_required(VERSION 3.15.0-rc1)
set(CMAKE_GENERATOR_PLATFORM x64)

project(VultureEngine)

add_subdirectory(engine)
add_subdirectory(editor)

set_property(DIRECTORY PROPERTY VS_STARTUP_PROJECT vul2_editor)