cmake_minimum_required(VERSION 3.13)

include(cmake/pico_sdk_import.cmake)

project(firmware C CXX ASM)
set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)
pico_sdk_init()

include_directories(${CMAKE_CURRENT_LIST_DIR}/include)
add_subdirectory(src)