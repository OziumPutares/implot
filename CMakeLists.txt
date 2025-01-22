cmake_minimum_required(VERSION 3.31)
project(CMakeSFMLProject LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
add_library(${PROJECT_NAME} implot.h implot.cpp)

set_target_properties(
  ${PROJECT_NAME}
  PROPERTIES CXX_STANDARD 23
             CXX_STANDARD_REQUIRED YES
             CXX_EXTENSIONS NO)
