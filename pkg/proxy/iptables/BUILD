package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["proxier.go"],
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/api/service:go_default_library",
        "//pkg/proxy:go_default_library",
        "//pkg/proxy/healthcheck:go_default_library",
        "//pkg/types:go_default_library",
        "//pkg/util/config:go_default_library",
        "//pkg/util/exec:go_default_library",
        "//pkg/util/flowcontrol:go_default_library",
        "//pkg/util/iptables:go_default_library",
        "//pkg/util/sets:go_default_library",
        "//pkg/util/slice:go_default_library",
        "//pkg/util/sysctl:go_default_library",
        "//vendor:github.com/coreos/go-semver/semver",
        "//vendor:github.com/davecgh/go-spew/spew",
        "//vendor:github.com/golang/glog",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["proxier_test.go"],
    library = "go_default_library",
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/proxy:go_default_library",
        "//pkg/types:go_default_library",
        "//pkg/util/exec:go_default_library",
        "//pkg/util/iptables:go_default_library",
        "//pkg/util/iptables/testing:go_default_library",
    ],
)
