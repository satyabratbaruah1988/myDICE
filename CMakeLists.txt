cmake_minimum_required(VERSION 3.15)

project(DICE_Crypto_Bundle LANGUAGES C)

enable_testing()

set(BUILD_QCBOR_TEST "APP" CACHE STRING "Build QCBOR tests")
set(BUILD_TESTS ON CACHE BOOL "Build t_cose tests")
set(CRYPTO_PROVIDER "TinyCrypt" CACHE STRING "t_cose crypto provider")
set(BUILD_EXAMPLES ON CACHE BOOL "Build t_cose examples")

add_subdirectory(QCBOR)
add_subdirectory(tinycrypt)
add_subdirectory(t_cose)
