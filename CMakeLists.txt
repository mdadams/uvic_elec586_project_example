# Specify the minimum required version of CMake.
cmake_minimum_required(VERSION 3.1 FATAL_ERROR)

# Specify the project and identify languages used.
project(project LANGUAGES CXX)

# Add program target called hello.
add_executable(hello hello.cpp)

# Add program target called goodbye.
add_executable(goodbye goodbye.cpp)

# Install the hello and goodbye programs.
install(TARGETS hello goodbye DESTINATION bin)

# Install the demo script.
install(PROGRAMS demo DESTINATION bin)
