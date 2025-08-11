cmake_minimum_required(VERSION 3.28)

project(opengl_class LANGUAGES CXX)

find_package(OpenGL REQUIRED)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

file(GLOB_RECURSE files "src/*.cpp")

add_executable(${PROJECT_NAME} ${files})

target_include_directories(${PROJECT_NAME} PUBLIC include)

add_subdirectory(dependencies/glfw-3.4 glfw)

target_link_libraries(${PROJECT_NAME} OpenGL::GL glfw )




