cmake_minimum_required(VERSION 3.15.0-rc1)

project(vul2_editor)

add_executable(${PROJECT_NAME} src/main.cpp)

set_property (DIRECTORY PROPERTY VS_STARTUP_PROJECT vul2_editor)

link_directories(${PROJECT_NAME} PRIVATE engine)

add_subdirectory(engine)

target_link_libraries(${PROJECT_NAME} vul2_engine)
