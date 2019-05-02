cmake_minimum_required(VERSION 3.10)
project(EEEL_Cmake)

set(CMAKE_CXX_STANDARD 11)
SET(CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -Wall -Wno-sign-compare -fno-builtin-malloc -fno-builtin-calloc -fno-builtin-realloc -fno-builtin-free -fno-omit-frame-pointer -DNDEBUG")

set(SOURCES src/analyst.cpp
        src/context.cpp
        src/ee_engine.cpp
        src/hierarchy.cpp
        src/node.cpp
        src/pl_math.cpp
        src/solver.cpp
        src/string_util.cpp
        src/util.cpp)

add_executable(main tools/ee_main.cpp ${SOURCES})
target_link_libraries(main pthread gflags glog)

add_executable(analysis tools/ee_analysis_main.cpp ${SOURCES})
target_link_libraries(analysis pthread gflags glog)