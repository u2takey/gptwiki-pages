# cargo rustc 
## chatgpt 
The `cargo rustc` command is used to build and compile Rust programs using the Rust Compiler (rustc) via the Cargo build system. The `cargo` tool is a build system and package manager for Rust which provides various utilities for managing Rust projects such as downloading, building, and deploying dependencies.

When using the `cargo rustc` command, Cargo will:

- Analyze the project’s dependencies
- Select the appropriate version of the Rust compiler (rustc) for the project
- Set up the environment for building the project
- Compile the project, generating an executable or library

You can also pass additional options to the `rustc` component by using `--` after the `cargo rustc` command. For example, `cargo rustc -- --emit=llvm-ir` will generate LLVM IR instead of object files. 

Overall, `cargo rustc` is an essential tool for Rust developers and provides an easy way to build and compile their projects. 

## tldr 
 
> Compile a Rust package, and pass extra options to the compiler.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-rustc.html>.

- Build the package or packages defined by the `Cargo.toml` manifest file in the current working directory:

`cargo rustc`

- Build artifacts in release mode, with optimizations:

`cargo rustc --release`

- Compile with architecture-specific optimizations for the current CPU:

`cargo rustc --release -- -C target-cpu=native`

- Compile with speed optimization:

`cargo rustc -- -C opt-level {{1|2|3}}`

- Compile with [s]ize optimization (`z` also turns off loop vectorization):

`cargo rustc -- -C opt-level {{s|z}}`

- Check if your package uses unsafe code:

`cargo rustc --lib -- -D unsafe-code`

- Build a specific package:

`cargo rustc --package {{package}}`

- Build only the specified binary:

`cargo --bin {{name}}`
