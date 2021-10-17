project(Fibonacci-Cmake)
cmake_minimum_required(VERSION 3.19.1)

set(HEADERS
    include/Matrix.h
    include/Vector.h
)

set(SOURCES
    src/Matrix.cpp
    src/Vector.cpp
    src/Source.cpp
)

add_executable(demo ${SOURCES} ${HEADERS})
target_include_directories(demo PUBLIC include)
