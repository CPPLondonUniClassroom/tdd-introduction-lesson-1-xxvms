cmake_minimum_required(VERSION 3.11)
project(TDD_Lesson1)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED 17)

option(DISABLE_TESTS "Disable compilation of unit tests" OFF)

add_subdirectory(src)
if (NOT DISABLE_TESTS)
    add_subdirectory(test)
endif()
