cmake_minimum_required(VERSION 3.15)
project(HW2)
set(CMAKE_CXX_STANDARD 17)

find_package(sfml)
find_package(OpenGL)
include_directories(${SFML_INCLUDE_DIRECTORIES})

add_executable(HW2 main.cpp)
target_link_libraries(HW2 PRIVATE sfml-system sfml-window sfml-graphics OpenGL)