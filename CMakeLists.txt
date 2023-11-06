cmake_minimum_required(VERSION 3.14)

if(${CMAKE_VERSION} VERSION_LESS 3.14)
    cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
endif()

project(plf_nanotimer)
add_library(plf_nanotimer INTERFACE
            plf_nanotimer.h            
)   

target_include_directories(plf_nanotimer INTERFACE ${CMAKE_INCLUDE_CURRENT_DIR})