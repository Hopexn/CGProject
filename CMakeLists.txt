cmake_minimum_required (VERSION 2.6)
project(OurCraft)
include_directories(OpenGL/include)
set(CMAKE_CXX_FLAGS "-g -Wall")
set(TARGET_LIB "freeglut_static.lib")
add_executable(OurCraft OurCraft/OurCraft.cpp OurCraft/param.h OurCraft/structs.h)
target_link_libraries(OurCraft ${TARGET_LIB})

