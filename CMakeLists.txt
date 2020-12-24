cmake_minimum_required(VERSION 3.17)
project(yacppclp)

set(CMAKE_CXX_STANDARD 17)

include("cmake_functions.txt")

# Set release build by default.
if(NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE RelWithDebInfo)
endif()

# if {fmt} exists and is not in a standard path,
# set "fmt_DIR" to the directory containing fmtConfig.cmake or fmt-config.cmake
import_fmtlib()
