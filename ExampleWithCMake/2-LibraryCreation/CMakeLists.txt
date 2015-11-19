project(Example)
cmake_minimum_required(VERSION 2.8)

add_library(shadok SHARED shadok.cpp)
install(TARGETS shadok DESTINATION lib)

add_executable(test main.cpp)
target_link_libraries(test shadok)

install(TARGETS test RUNTIME DESTINATION bin)




