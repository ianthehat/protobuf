workspace(name = "com_github_gogo_protobuf")

http_archive(
    name = "io_bazel_rules_go",
    url = "https://codeload.github.com/ianthehat/rules_go/zip/cca4472b4ecac6e20dcc2bb2a59b7260e3266d9d",
    strip_prefix = "rules_go-cca4472b4ecac6e20dcc2bb2a59b7260e3266d9d",
    type = "zip",
)

load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains")
load("@io_bazel_rules_go//proto:def.bzl", "proto_register_toolchains")
go_rules_dependencies()
go_register_toolchains()
register_toolchains(
    "@io_bazel_rules_go//proto:proto",
    "//:gogo",
    "//:gogo_grpc",
)
proto_register_toolchains()
