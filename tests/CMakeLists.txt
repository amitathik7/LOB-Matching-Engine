add_executable(lob_tests basic_test.cpp)
target_link_libraries(lob_tests PRIVATE lob_library GTest::gtest_main)

include(GoogleTest)
gtest_discover_tests(lob_tests)