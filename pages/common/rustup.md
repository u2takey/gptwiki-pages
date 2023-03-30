# rustup 
## chatgpt 
Rustup is a command-line tool that is used for managing multiple installations of the Rust compiler on a single machine. When executed in a terminal, the Rustup command initializes the Rust toolchain and installs the latest stable version of the Rust compiler.

Rustup is also used for managing multiple toolchains of Rust, where each toolchain includes a specific version of the Rust compiler, along with a set of associated tools such as cargo (the Rust package manager) and rustfmt (the Rust code formatter).

The Rustup command is used to perform a variety of operations, such as installing and uninstalling Rust toolchains, managing components (such as additional Rust targets), updating Rust and its components to the latest version, and configuring the PATH environment variable to make Rust commands and tools available system-wide.

Rustup provides a convenient way to switch between different versions of the Rust toolchain and manage dependencies required for specific projects. Overall, it simplifies the process of working with Rust and ensures that everything required to build, run and test Rust code is always available on your machine. 

## tldr 
 
> Rust toolchain installer.
> Install, manage, and update Rust toolchains.
> More information: <https://github.com/rust-lang/rustup.rs>.

- Install the nightly toolchain for your system:

`rustup install nightly`

- Switch the default toolchain to nightly so that the `cargo` and `rustc` commands will use it:

`rustup default nightly`

- Use the nightly toolchain when inside the current project, but leave global settings unchanged:

`rustup override set nightly`

- Update all toolchains:

`rustup update`

- List installed toolchains:

`rustup show`

- Run cargo build with a certain toolchain:

`rustup run {{toolchain_name}} cargo build`

- Open the local rust documentation in the default web browser:

`rustup doc`
