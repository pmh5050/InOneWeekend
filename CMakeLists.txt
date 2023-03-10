cmake_minimum_required(VERSION 3.14.0)
project(InOneWeekend)

# find_package()

set(INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include)
set(SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)

file(GLOB_RECURSE SOURCES
    "${INCLUDE_DIR}/*.h"
    "${SOURCE_DIR}/*.cpp"
)

add_executable(${PROJECT_NAME} ${SOURCES})