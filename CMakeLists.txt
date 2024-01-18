cmake_minimum_required(VERSION 3.28.1)

project(IG_API)


set(CURL_DIR "D:/Study/C++/Dev_Tools/curl-8.5.0")

include_directories(${CURL_DIR}/include)

add_executable(main main.cpp)

find_library(CURL_LIB NAMES libcurl PATHS ${CURL_DIR}/lib)
target_link_libraries(main ${CURL_LIB})



