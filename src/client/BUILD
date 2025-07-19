load("@crates//:defs.bzl", "all_crate_deps")
load("@rules_rust//rust:defs.bzl", "rust_binary")

rust_binary(
    name = "client",
    srcs = glob(["src/**/*.rs"]),
    platform = "@rules_rust//rust/platform:wasm32",
    visibility = ["//visibility:public"],
    deps = all_crate_deps(proc_macro = False),
)
