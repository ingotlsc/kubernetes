package(default_visibility = ["//visibility:public"])

licenses(["notice"])

filegroup(
    name = "package-srcs",
    srcs = glob(
        ["**"],
        exclude = [
            "etcd*/**",
            "etcd*.tar.gz",
        ],
    ),
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//third_party/forked/golang/expansion:all-srcs",
        "//third_party/forked/golang/net:all-srcs",
        "//third_party/forked/golang/reflect:all-srcs",
        "//third_party/forked/golang/template:all-srcs",
        "//third_party/forked/gonum/graph:all-srcs",
    ],
    tags = ["automanaged"],
)
