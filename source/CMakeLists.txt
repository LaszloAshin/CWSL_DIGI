cmake_minimum_required(VERSION 3.10)
project(CWSL_DIGI VERSION 0.88 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt6 REQUIRED COMPONENTS Core)
qt_standard_project_setup()

qt_add_executable(CWSL_DIGI CWSL_DIGI.cpp)
target_link_libraries(CWSL_DIGI PRIVATE Qt6::Core)
