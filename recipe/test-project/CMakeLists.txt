cmake_minimum_required(VERSION 3.16)

project(test-metatensor CXX)

find_package(metatensor)

add_executable(main main.cpp)
target_link_libraries(main metatensor)

enable_testing()
add_test(NAME main COMMAND main)
