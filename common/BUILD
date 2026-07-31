load("@protobuf//bazel:cc_proto_library.bzl", "cc_proto_library")
load("@protobuf//bazel:proto_library.bzl", "proto_library")

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

proto_library(
    name = "packageinventory_proto",
    srcs = ["packageinventory.proto"],
    visibility = ["//visibility:public"],
    deps = ["@protobuf//:duration_proto"],
)

cc_proto_library(
    name = "packageinventory_cc_proto",
    deps = [":packageinventory_proto"],
    visibility = ["//visibility:public"],
)
