# Bazel Rust Project

This is a Bazel workspace configured for Rust development. It demonstrates the integration between Bazel build system and Rust/Cargo.

## Project Structure

- `WORKSPACE`: Contains Bazel workspace configuration and external dependencies
- `src/client`: A sample Rust crate
- `.bazelrc`: Bazel configuration file

## Building

To build the project:

```bash
bazel build //src/client
```

To run the hello world example:

```bash
bazel run //src/client
```

## Development

This project uses Bazel for build management while maintaining compatibility with Cargo. You can use either build system:

- Use `bazel build //...` to build all targets
- Use `cargo build` in individual crate directories for Cargo builds
