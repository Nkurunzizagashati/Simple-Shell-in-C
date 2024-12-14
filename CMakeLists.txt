cmake_minimum_required(VERSION 3.10)

# Set project name
project(SimpleShell C)

# Set CXX compiler to empty string (avoid C++ detection)
set(CMAKE_CXX_COMPILER "")

# Set C Compiler flags
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Wextra -g")

# Include directories (header files)
include_directories(include)

# Define source files
set(SRC_FILES src/main.c )

# Create the executable
add_executable(simple_shell ${SRC_FILES})
