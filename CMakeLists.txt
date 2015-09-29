cmake_minimum_required(VERSION 3.1)

project(JCudaMain)

include(${CMAKE_CURRENT_SOURCE_DIR}/../jcuda-common/JCudaCommon_CMake.txt)

add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/../JCuda/src/main/native/driver
    ${CMAKE_CURRENT_BINARY_DIR}/JCuda/JCudaDriverJNI/bin)
    
add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/../JCuda/src/main/native/runtime
    ${CMAKE_CURRENT_BINARY_DIR}/JCuda/JCudaRuntimeJNI/bin)
    
add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/../JCublas/src/main/native/cublas
    ${CMAKE_CURRENT_BINARY_DIR}/JCublas/JCublasJNI/bin)
