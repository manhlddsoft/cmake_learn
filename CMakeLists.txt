cmake_minimum_required(VERSION 3.10)
project(cmake_learn)

set(PROJECT_INCLUDE_FILES 
    ${CMAKE_SOURCE_DIR}/inc/)

add_executable(${PROJECT_NAME}
    ${CMAKE_SOURCE_DIR}/src/main.c)

target_include_directories(${PROJECT_NAME} PRIVATE
    ${PROJECT_INCLUDE_FILES})