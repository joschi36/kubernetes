load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["interface.go"],
    importmap = "k8s.io/kubernetes/vendor/k8s.io/sample-apiserver/pkg/client/informers/externalversions/wardle",
    importpath = "k8s.io/sample-apiserver/pkg/client/informers/externalversions/wardle",
    visibility = ["//visibility:public"],
    deps = [
        "//staging/src/k8s.io/sample-apiserver/pkg/client/informers/externalversions/internalinterfaces:go_default_library",
        "//staging/src/k8s.io/sample-apiserver/pkg/client/informers/externalversions/wardle/v1alpha1:go_default_library",
        "//staging/src/k8s.io/sample-apiserver/pkg/client/informers/externalversions/wardle/v1beta1:go_default_library",
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
        "//staging/src/k8s.io/sample-apiserver/pkg/client/informers/externalversions/wardle/v1alpha1:all-srcs",
        "//staging/src/k8s.io/sample-apiserver/pkg/client/informers/externalversions/wardle/v1beta1:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
