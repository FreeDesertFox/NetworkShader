cmake_minimum_required(VERSION 3.10.0)
project(NetworkShader VERSION 0.1.0 LANGUAGES C CXX)

include_directories(lib/asio/asio/include)

add_subdirectory(src)

