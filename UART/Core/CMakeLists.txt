cmake_minimum_required(VERSION 3.10)  
project(MyProject)  

set(CMAKE_CXX_STANDARD 11)  
set(CMAKE_CXX_STANDARD_REQUIRED ON)  

include_directories(${PROJECT_SOURCE_DIR}/include)  
aux_source_directory(${PROJECT_SOURCE_DIR}/src SRC_FILES)  

add_executable(MyExecutable ${SRC_FILES})
