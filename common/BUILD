load("@protobuf//bazel:cc_proto_library.bzl", "cc_proto_library")

licenses(["notice"])

proto_library(
    name = "signals_proto",
    srcs = ["signals.proto"],
    visibility = ["//visibility:public"],
    deps = [],
)

cc_proto_library(
    name = "signals_cc_proto",
    deps = [":signals_proto"],
    visibility = ["//visibility:public"],
)
