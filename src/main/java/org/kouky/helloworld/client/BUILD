java_binary(
    name = "helloworld_client_simulator",
    main_class = "org.kouky.helloworld.client.HelloWorldClient",
    visibility = [
        "//visibility:public",
    ],
    runtime_deps = [
        ":helloworld_client",
    ],
)

java_library(
    name = "helloworld_client",
    srcs = glob(["*.java"]),
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
