load("@protobuf//bazel:cc_proto_library.bzl", "cc_proto_library")

proto_library(
    name = "v1_proto",
    srcs = ["v1.proto"],
    deps = [
        "@protobuf//:timestamp_proto",
    ],
    visibility = ["//visibility:public"],
)

cc_proto_library(
    name = "v1_cc_proto",
    deps = [":v1_proto"],
    visibility = ["//visibility:public"],
)

