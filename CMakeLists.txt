cmake_minimum_required(VERSION 3.26 FATAL_ERROR)

project(cmake
    VERSION         0.0.1
    DESCRIPTION     "jun's CMake demo"
    HOMEPAGE_URL    "https://github.com/yu-niao/cmake"
    LANGUAGES       C CXX
)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(BuildInfo)

add_subdirectory(external)

add_subdirectory(src)

add_subdirectory(docs)

add_subdirectory(test)

add_subdirectory(packaging)