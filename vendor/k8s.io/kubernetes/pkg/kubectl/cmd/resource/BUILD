load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["get.go"],
    importpath = "k8s.io/kubernetes/pkg/kubectl/cmd/resource",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/spf13/cobra:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/meta:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1/unstructured:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/cmd/templates:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/cmd/util:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/cmd/util/openapi:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/resource:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/util/i18n:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/printers:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/util/interrupt:go_default_library",
    ],
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
