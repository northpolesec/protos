load("@rules_cc//cc:defs.bzl", "cc_proto_library")
load("@rules_go//proto:def.bzl", "go_proto_library")

licenses(["notice"])

proto_library(
    name = "sync_v1_proto",
    srcs = ["syncv1.proto"],
)

cc_proto_library(
    name = "sync_v1_cc_proto",
    deps = [":sync_v1_proto"],
)

go_proto_library(
    name = "sync_v1_go_proto",
    importpath = "github.com/northpolesec/protos/sync_v1_proto",
    protos = [":sync_v1_proto"],
)
