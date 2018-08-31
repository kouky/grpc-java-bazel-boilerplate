java_binary(
    name = "helloworld_server",
    main_class = "org.kouky.helloworld.server.HelloWorldServer",
    visibility = [
        "//visibility:public",
    ],
    runtime_deps = [
        ":helloworld_serve_lib",
    ],
)

java_library(
    name = "helloworld_serve_lib",
    srcs = glob(["*.java"]),
    deps = [
        "//3rdparty/jvm/io/grpc:grpc_stub",
        "//3rdparty/jvm/io/grpc:grpc_netty",
        "//3rdparty/jvm/io/grpc:grpc_protobuf",
        "//src/main/proto:helloworld_java_proto",
        "//src/main/proto:helloworld_java_grpc",
    ],
)
