# gRPC Java Bazel Boilerplat

Boilerplate for commencing a new Java based [gRPC](https://grpc.io) microservices project using the [Bazel](https://bazel.build build) system.

## Managing Third Party Dependencies

Third party dependencies are specified in `dependencies.yaml` and generated by [bazel-deps](https://github.com/johnynek/bazel-deps).

To update or regenerate `3rdparty` dependencies clone the `bazel-deps` repo, change directory into it, and run the following.

```
bazel run //:parse -- generate -r /path/to/grpc-java-bazel-boilerplate -s 3rdparty/workspace.bzl -d dependencies.yaml
```