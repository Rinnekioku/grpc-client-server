cmake_minimum_required(VERSION 3.23)
project(server)

add_executable(server main.cpp)

target_link_libraries(server rg_grpc_proto grpc++_reflection libprotobuf grpc++ helper)
