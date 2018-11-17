package(default_visibility = ["//visibility:public"])

load("@org_pubref_rules_protobuf//cpp:rules.bzl", "cc_proto_library")
load("@org_pubref_rules_protobuf//python:rules.bzl", "py_proto_library")
load("@org_pubref_rules_protobuf//protobuf:rules.bzl", "proto_compile")

filegroup(
    name = "protos",
    srcs = [
        "common.proto",
    ],
)

cc_proto_library(
    name = "cpp",
    protos = [":protos"],
)

py_proto_library(
    name = "py",
    protos = [":protos"],
    verbose = 0,
    with_grpc = False,
)