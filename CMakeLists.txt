cmake_minimum_required(VERSION 3.17)
project(Google_tests)

add_subdirectory(Libni)
add_subdirectory(googletest)
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})
# adding the Google_Tests_run target

add_executable(Google_Tests_run test.cpp)


target_link_libraries(Google_Tests_run gtest gtest_main Libni)