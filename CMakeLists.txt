cmake_minimum_required(VERSION 3.16)

if(CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_SOURCE_DIR)
    project(sht31d CXX)
endif()

add_library(sht31d STATIC
    "${CMAKE_CURRENT_SOURCE_DIR}/src/ClosedCube_SHT31D.cpp"
)
target_include_directories(sht31d PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")
