cmake_minimum_required(VERSION 3.1)

project(JCudaMain)

include(${CMAKE_CURRENT_SOURCE_DIR}/../jcuda-common/JCudaCommon_CMake.txt)

add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/../JCuda/JCudaDriverJNI
    ${CMAKE_CURRENT_BINARY_DIR}/JCuda/JCudaDriverJNI/bin)
    
add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/../JCuda/JCudaRuntimeJNI
    ${CMAKE_CURRENT_BINARY_DIR}/JCuda/JCudaRuntimeJNI/bin)
    
add_subdirectory(
    ${CMAKE_CURRENT_SOURCE_DIR}/../JCublas/JCublasJNI
    ${CMAKE_CURRENT_BINARY_DIR}/JCublas/JCublasJNI/bin)
