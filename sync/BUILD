load("@rules_cc//cc:defs.bzl", "cc_proto_library")
load("@rules_go//proto:def.bzl", "go_proto_library")

licenses(["notice"])

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

go_proto_library(
    name = "v1_go_proto",
    importpath = "github.com/northpolesec/protos/sync/v1_proto",
    protos = [":v1_proto"],
    visibility = ["//visibility:public"],
)
