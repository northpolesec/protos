load("@rules_cc//cc:defs.bzl", "cc_proto_library")
load("@rules_go//proto:def.bzl", "go_proto_library")

proto_library(
    name = "v1_proto",
    srcs = ["v1.proto"],
    deps = [
        "@protobuf//:any_proto",
        "@protobuf//:timestamp_proto",
    ],
    visibility = ["//visibility:public"],
)

cc_proto_library(
    name = "v1_cc_proto",
    deps = [":v1_proto"],
    visibility = ["//visibility:public"],
)

# Note: Simple wrapper for a `cc_proto_library` target which cannot be directly
# depended upon by an `objc_library` target.
cc_library(
    name = "cc_proto_library_wrapper",
    hdrs = ["proto_include_wrapper.h"],
    deps = [
        ":v1_cc_proto",
    ],
    visibility = ["//visibility:public"],
)

go_proto_library(
    name = "v1_go_proto",
    importpath = "github.com/northpolesec/protos/telemetry/v1_proto",
    protos = [":v1_proto"],
    visibility = ["//visibility:public"],
)

