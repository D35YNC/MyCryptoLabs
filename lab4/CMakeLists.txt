cmake_minimum_required(VERSION 3.5)

project(lab4 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGSS} -std=c++20")

add_executable(lab4 main.cpp)
target_include_directories(lab4 PUBLIC "${CMAKE_SOURCE_DIR}/mycryptolib/")
target_link_libraries(lab4 mycryptolib)
