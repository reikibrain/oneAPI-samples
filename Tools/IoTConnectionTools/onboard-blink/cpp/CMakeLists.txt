set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${MRAA_CFLAGS}")
add_executable (blink blink.cpp)
add_custom_target (run ./blink)
target_link_libraries(blink ${MRAA_LDFLAGS})
