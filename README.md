# example-bazel-cargo-wasm-with-tokio

An example of using Rust target triples to allow bazel to compile a project with Linux and WASM targets with tokio platform dependencies.

Adding non-wasm dependencies under `[target.'cfg(not(target_arch = "wasm32"))'.dependencies]` in the `Cargo.toml` file will ensure they are only included in the Linux build.

ex:

```toml
[target.'cfg(not(target_arch = "wasm32"))'.dependencies]
tokio = { workspace = true, features = ["full"] }
```

## Building

To build projects:

```bash
bazel build //...
```
