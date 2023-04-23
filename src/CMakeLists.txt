cmake_minimum_required(VERSION 3.8)
project(QtExample CXX)

set(CMAKE_AUTOMOC ON)
set(CMAKE_INCLUDE_CURRENT_DIR ON)
find_package(Qt5 COMPONENTS Core Widgets REQUIRED)

add_executable(qtexample qtexample.cpp window.cpp window.hpp)
target_link_libraries(qtexample Qt5::Widgets)
