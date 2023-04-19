cmake_minimum_required(VERSION 3.20)
project(learning VERSION 1.0)
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# which is the executable - doesn't have to be just the executable file
add_executable(tutorial tutorial.cxx)

configure_file(TutorialConfig.h.in TutorialConfig.h)

# this tells where to look for headers
target_include_directories(tutorial PUBLIC "${PROJECT_BINARY_DIR}")
