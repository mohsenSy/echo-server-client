cmake_minimum_required(VERSION 2.8.12)
project(ctest)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()


add_executable(ctest src/main.c)

add_executable(server src/server.c)
add_executable(client src/client.c)

target_link_libraries(server ${CONAN_LIBS})
target_link_libraries(client ${CONAN_LIBS})
target_link_libraries(ctest ${CONAN_LIBS})
