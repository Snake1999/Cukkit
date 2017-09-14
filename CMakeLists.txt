cmake_minimum_required(VERSION 3.8)
project(levitate)

set(CMAKE_CXX_STANDARD 17)

set(Boost_Path "E:/boost_1_65_1")
set(Boost_INCLUDE_DIR "${Boost_Path}")
find_package(Boost 1.65.1)
if(Boost_FOUND)
    include_directories(${Boost_INCLUDE_DIRS})
endif()

set(SOURCE_FILES Cukkit.cpp)
add_executable(Cukkit ${SOURCE_FILES})