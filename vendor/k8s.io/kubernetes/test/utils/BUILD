load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "conditions.go",
        "density_utils.go",
        "deployment.go",
        "pod_store.go",
        "replicaset.go",
        "runners.go",
        "tmpdir.go",
    ],
    importpath = "k8s.io/kubernetes/test/utils",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/davecgh/go-spew/spew:go_default_library",
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/k8s.io/api/batch/v1:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/api/extensions/v1beta1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/equality:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/fields:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/uuid:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/client-go/scale:go_default_library",
        "//vendor/k8s.io/client-go/tools/cache:go_default_library",
        "//vendor/k8s.io/client-go/util/workqueue:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/v1/pod:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/batch:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/extensions:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/client/clientset_generated/internalclientset:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/controller/deployment/util:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/util/labels:go_default_library",
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
        "//vendor/k8s.io/kubernetes/test/utils/image:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
