cmake_minimum_required(VERSION 3.10.0)
project(NetworkShader VERSION 0.1.0 LANGUAGES C CXX)

find_package(OpenSSL REQUIRED)

if(NOT OPENSSL_FOUND)
    message(FATAL_ERROR "Need OPENSSL library for safety connection")
endif()

include_directories(${OPENSSL_INCLUDE_DIR})

include_directories(lib/asio/asio/include)

add_subdirectory(src)

