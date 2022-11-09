cmake_minimum_required(VERSION 3.23)
project(client)

add_executable(client main.cpp)

target_link_libraries(client rg_grpc_proto grpc++_reflection libprotobuf grpc++ helper)
