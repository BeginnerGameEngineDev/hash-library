cmake_minimum_required (VERSION 3.24.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

project(hash-lib)

add_library(hash-library crc32.h crc32.cpp digest.cpp hash.h hmac.h keccak.h keccak.cpp md5.h md5.cpp sha1.h sha1.cpp sha3.h sha3.cpp sha256.h sha256.cpp)
target_include_directories(hash-library PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/)
