cmake_minimum_required(VERSION 2.8)
project(easywsclient)

set(CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake_modules" ${CMAKE_MODULE_PATH})
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
set(DEFAULT_FLAGS "-pthread -std=c++14 -Wall -Werror -Wno-unused-result -Wno-unknown-pragmas")

add_library(easywsclient_lib easywsclient.cpp easywsclient.hpp)
