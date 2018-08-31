java_binary(
    name = "helloworld_server",
    srcs = glob(["*.java"]),
    main_class = "org.kouky.helloworld.server.HelloWorldServer",
    visibility = [
        "//visibility:public",
    ],
    deps = [
        "//3rdparty/jvm/io/grpc:grpc_stub",
        "//3rdparty/jvm/io/grpc:grpc_netty",
        "//3rdparty/jvm/io/grpc:grpc_protobuf",
        "//src/main/proto:helloworld_java_proto",
        "//src/main/proto:helloworld_java_grpc",
    ],
)
