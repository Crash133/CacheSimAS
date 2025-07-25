cmake_minimum_required(VERSION 3.31)
project(CacheSimAS)

#Include the directories and now your cpp files will recognize your headers
include_directories(${CMAKE_SOURCE_DIR}/include)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(CMAKE_CXX_STANDARD 20)

add_executable(CacheSimAS main.cpp
        Cache.cpp
        include/Cache.h
        CacheSimulator.cpp
        include/CacheSimulator.h)
