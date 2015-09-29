cmake_minimum_required(VERSION 3.1)

project(JCuda)

include(${CMAKE_CURRENT_SOURCE_DIR}/../jcuda-common/JCudaCommon_CMake.txt)

add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/src/main/native/driver
    ${CMAKE_CURRENT_BINARY_DIR}/JCuda/JCudaDriverJNI/bin)
    
add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/src/main/native/runtime
    ${CMAKE_CURRENT_BINARY_DIR}/JCuda/JCudaRuntimeJNI/bin)