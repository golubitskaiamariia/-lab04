cmake_minimum_required(VERSION 3.5)

project(formatter_ex)

add_library(formatter_ex STATIC formatter_ex.cpp)
target_include_directories(formatter_ex PUBLIC 
    ${CMAKE_CURRENT_SOURCE_DIR}
    ${CMAKE_SOURCE_DIR}/formatter_lib
)

target_link_libraries(formatter_ex PRIVATE formatter)
