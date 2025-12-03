load("@protobuf//bazel:cc_proto_library.bzl", "cc_proto_library")

proto_library(
    name = "v2_proto",
    srcs = ["v2.proto"],
    deps = [
        "@protobuf//:timestamp_proto",
    ],
    visibility = ["//visibility:public"],
)

cc_proto_library(
    name = "v2_cc_proto",
    deps = [":v2_proto"],
    visibility = ["//visibility:public"],
)

