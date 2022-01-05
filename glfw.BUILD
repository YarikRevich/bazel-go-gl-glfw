load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "imgui-go",
    srcs = glob(["*.cpp", "*.go", "*.h"], ["*_test.go"]),
    importpath = "github.com/inkyblackness/imgui-go/v2",
    cgo = True,
    cdeps = ["@org_freetype_freetype2//:freetype2"],
    visibility = ["//visibility:public"],
)

alias(
    name = "go_default_library",
    actual = ":imgui-go",
    visibility = ["//visibility:public"],
)
