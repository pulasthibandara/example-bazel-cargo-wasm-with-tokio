load("@crates//:defs.bzl", "all_crate_deps")
load("@rules_rust//rust:defs.bzl", "rust_binary")

rust_binary(
    name = "server",
    srcs = glob(["src/**/*.rs"]),
    visibility = ["//visibility:public"],
    deps = all_crate_deps(proc_macro = False),
)
