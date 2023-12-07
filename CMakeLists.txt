cmake_minimum_required(VERSION 3.26)
project(Sorting_Visualizer_With_CPP)



set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -lmingw32")
set(CMAKE_EXE_LINKER_FLAGS "-static-libgcc -static-libstdc++")

include_directories(${PROJECT_SOURCE_DIR}/include)
link_directories(${PROJECT_SOURCE_DIR}/lib)

set(SOURCE_FILES main.cpp)
add_executable(Sorting_Visualizer_With_CPP ${SOURCE_FILES})

target_link_libraries(Sorting_Visualizer_With_CPP mingw32 SDL2main SDL2)