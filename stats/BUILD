load("@grpc//bazel:cc_grpc_library.bzl", "cc_grpc_library")
load("@protobuf//bazel:cc_proto_library.bzl", "cc_proto_library")

proto_library(
    name = "v1_proto",
    srcs = ["v1.proto"],
    visibility = ["//visibility:public"],
)

cc_proto_library(
    name = "v1_cc_proto",
    deps = [":v1_proto"],
    visibility = ["//visibility:public"],
)

cc_grpc_library(
    name = "v1_cc_grpc",
    srcs = [
        ":v1_proto",
    ],
    grpc_only = True,
    deps = [
        ":v1_cc_proto",
    ],
    visibility = ["//visibility:public"],
)
