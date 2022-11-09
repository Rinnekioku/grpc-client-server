cmake_minimum_required(VERSION 3.23)
project(helper)

add_library(helper
        SHARED
        helper.cpp)

target_include_directories(helper
        PUBLIC
        .)

target_link_libraries(helper grpc++_reflection grpc++ libprotobuf rg_grpc_proto)
