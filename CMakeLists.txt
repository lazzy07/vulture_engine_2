cmake_minimum_required(VERSION 3.15.0-rc1)

project(VultureEditor)

add_executable(${PROJECT_NAME} editor/src/main.cpp)

target_link_directories(${PROJECT_NAME} PRIVATE engine)

add_subdirectory(engine)

target_link_libraries(${PROJECT_NAME} engine)