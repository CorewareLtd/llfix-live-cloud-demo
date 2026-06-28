cmake_minimum_required(VERSION 3.8)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
project(demo_clients LANGUAGES CXX)

include("../../llfix.cmake")

add_executable(demo_clients clients.cpp)

configure_llfix(demo_clients)

configure_file(config.cfg config.cfg COPYONLY)
