cmake_minimum_required(VERSION 3.1)
project(imgEnhancement)
find_package(OpenCV REQUIRED)

include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable(BBHE BBHE.cpp)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
set(CMAKE_CXX_EXTENSIONS OFF)

target_link_libraries(BBHE ${OpenCV_LIBS})
