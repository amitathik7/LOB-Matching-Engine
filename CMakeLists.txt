cmake_minimum_required(VERSION 4.4.5)
project(lob_matching_engine LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED YES)
set(CMAKE_CXX_EXTENSIONS NO)

include(FetchContent)
FetchContent_Declare(googletest GIT_REPOSITORY https://github.com/google/googletest.git GIT_TAG v1.17.0)
FetchContent_MakeAvailable(googletest)

enable_testing()
add_subdirectory(src)
add_subdirectory(tests)