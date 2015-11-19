project(Example)
cmake_minimum_required(VERSION 2.8)

add_library(shadok SHARED shadok.cpp)
install(TARGETS shadok DESTINATION lib)


