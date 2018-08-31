load("//:java_grpc_library.bzl", "java_grpc_library")

proto_library(
    name = "helloworld_proto",
    srcs = ["helloworld.proto"],
)

java_proto_library(
    name = "helloworld_java_proto",
    deps = [":helloworld_proto"],
    visibility = ["//visibility:public"],
)

java_grpc_library(
    name = "helloworld_java_grpc",
    srcs = [":helloworld_proto"],
    deps = [":helloworld_java_proto"],
    visibility = ["//visibility:public"],
)
