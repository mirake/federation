load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "factory.go",
        "provider.go",
        "types.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/security/podsecuritypolicy",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/validation/field:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/extensions:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/apparmor:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/capabilities:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/group:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/seccomp:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/selinux:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/sysctl:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/user:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/util:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/securitycontext:go_default_library",
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
    srcs = [
        ":package-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/apparmor:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/capabilities:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/group:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/seccomp:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/selinux:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/sysctl:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/user:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/security/podsecuritypolicy/util:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
