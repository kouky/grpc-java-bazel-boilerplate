load("//3rdparty:workspace.bzl", "maven_dependencies")

maven_dependencies()

# proto_library, cc_proto_library, and java_proto_library rules implicitly
# depend on @com_google_protobuf for protoc and proto runtimes.
# This statement defines the @com_google_protobuf repo.
http_archive(
    name = "com_google_protobuf",
    sha256 = "d7a221b3d4fb4f05b7473795ccea9e05dab3b8721f6286a95fffbffc2d926f8b",
    strip_prefix = "protobuf-3.6.1",
    urls = ["https://github.com/google/protobuf/archive/v3.6.1.zip"],
)

# Archive of gRPC Java github repo. Used to access the C++ source code
# for the gRPC Java Codegen Plugin for Protobuf Compiler.
# See https://github.com/grpc/grpc-java/tree/master/compiler
# See java_grpc_library.bzl
http_archive(
    name = "io_grpc_archive",
    sha256 = "657ee70cbbc7e8c5aa26d622329f5fc8bfa6ce5e960bcdbff802f785b0eba212",
    strip_prefix = "grpc-java-1.14.0",
    urls = ["https://github.com/grpc/grpc-java/archive/v1.14.0.zip"],
)
