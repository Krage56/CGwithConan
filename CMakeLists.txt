cmake_minimum_required(VERSION 3.17)
project(OpenGLTest)

set(CMAKE_CXX_STANDARD 17)
include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()
add_executable(OpenGLTest main.cpp)
target_link_libraries(OpenGLTest ${CONAN_LIBS})