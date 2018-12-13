cmake_minimum_required(VERSION 3.12)
project(cppreactive)

set(CMAKE_CXX_STANDARD 17)
include(FetchContent)
include(RxCpp.cmake)

add_executable(cppreactive main.cpp)
target_link_libraries(cppreactive RxCpp)
target_include_directories(cppreactive PUBLIC ${rxcpp_SOURCE_DIR}/Rx/v2/src)
