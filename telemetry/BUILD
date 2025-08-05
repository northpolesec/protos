load("@protobuf//bazel:cc_proto_library.bzl", "cc_proto_library")

licenses(["notice"])

proto_library(
    name = "v1_proto",
    srcs = ["v1.proto"],
    visibility = ["//visibility:public"],
    deps = [
        "@protobuf//:any_proto",
        "@protobuf//:timestamp_proto",
    ],
)

cc_proto_library(
    name = "v1_cc_proto",
    deps = [":v1_proto"],
    visibility = ["//visibility:public"],
)

