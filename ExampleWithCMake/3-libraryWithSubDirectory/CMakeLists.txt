project(Example)
cmake_minimum_required(VERSION 2.8)

include_directories(shadok)

add_executable(test main.cpp)
target_link_libraries(test shadok)

install(TARGETS test RUNTIME DESTINATION bin)

add_subdirectory(shadok)



