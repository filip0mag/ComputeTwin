cmake_minimum_required(VERSION 3.20)

project(ComputeTwin
    VERSION 0.1.0
    LANGUAGES CXX
)

set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_executable(ComputeTwin
    src/main.cpp
)

target_compile_features(ComputeTwin PRIVATE cxx_std_20)

target_compile_options(ComputeTwin PRIVATE
    -Wall
    -Wextra
    -Wpedantic
)