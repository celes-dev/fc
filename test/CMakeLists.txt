add_subdirectory( crypto )
add_subdirectory( static_variant )
add_subdirectory( variant )

add_executable( test_base64 test_base64.cpp )
target_link_libraries( test_base64 fc )

add_test(NAME test_base64 COMMAND libraries/fc/test/test_base64 WORKING_DIRECTORY ${CMAKE_BINARY_DIR})
