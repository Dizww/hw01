#message(FATAL_ERROR "请修改 stbiw/CMakeLists.txt！要求生成一个名为 stbiw 的库")
cmake_minimum_required(VERSION 3.12)
project(stbiw LANGUAGES CXX)

add_library(stbiw STATIC stb_image_write.cpp stb_image_write.h)

target_include_directories(stbiw PUBLIC .)
