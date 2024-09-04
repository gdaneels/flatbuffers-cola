cmake_minimum_required(VERSION 3.10)
project(flatbuffers-cola)

set(CMAKE_C_STANDARD 11)

set(INC_DIR "${CMAKE_CURRENT_SOURCE_DIR}/include")
set(GEN_DIR "${CMAKE_CURRENT_SOURCE_DIR}/generated")
set(FBS_DIR "${CMAKE_CURRENT_SOURCE_DIR}/schemes")

include_directories("${GEN_DIR}" "${INC_DIR}")

add_executable(cola src/main.c)
target_link_libraries(cola "/home/gdaneels/workspace/flatbuffers/flatbuffers-cola/lib/libflatccrt.a")
