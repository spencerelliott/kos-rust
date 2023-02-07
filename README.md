## KallistiOS Rust Tool

`kos-rust` is a tool developed to help generate a Makefile for GCCRS Rust projects targeting the Sega Dreamcast. Because
the standard `cargo` command and Rust toolchain do not work natively with GCCRS, an alternative method using a Makefile
is the easiest way to build an executable ELF file.

This tool will read the dependencies from a project's `Cargo.toml` file, as well as the project's source, and generate
a Makefile in the `out/` directory of the project.

## Install

`kos-rust` can be installed using `cargo` on the host's computer

```shell
cargo install --git https://github.com/spencerelliott/kos-rust.git
```

## Usage

### Generating a Makefile

```shell
kos-rust generate
```

### Building a project

```shell
kos-rust build
```