load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["semver.go"],
    importmap = "k8s.io/kubernetes/vendor/golang.org/x/tools/internal/semver",
    importpath = "golang.org/x/tools/internal/semver",
    visibility = ["//vendor/golang.org/x/tools:__subpackages__"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
