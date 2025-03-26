cmake_minimum_required (VERSION 3.30)

project(GameEngine)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_executable(GameEngine 
    ${CMAKE_SOURCE_DIR}/src/Main.cpp
    ${CMAKE_SOURCE_DIR}/src/glad.c
)

target_include_directories(GameEngine PUBLIC
    ${CMAKE_SOURCE_DIR}/deps/include
    ${CMAKE_SOURCE_DIR}/include
)

target_link_directories(GameEngine PUBLIC
    ${CMAKE_SOURCE_DIR}/deps/lib
)

target_link_libraries(GameEngine PUBLIC
    glfw3
    opengl32
)
