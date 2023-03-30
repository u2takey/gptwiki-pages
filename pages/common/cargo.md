# cargo 
## chatgpt 
"Cargo" is a command-line tool used for managing Rust projects. It is the official Rust package manager, and it is used for building, testing, and publishing Rust libraries and applications. 

When you run the "cargo" command, it displays a list of subcommands that allows you to interact with your project. Some of the most commonly used subcommands include:

- "new" - creates a new Rust project
- "build" - compiles the current project
- "run" - compiles and runs the current project
- "test" - runs the tests in the current project
- "doc" - generates documentation for the current project
- "publish" - publishes the current project to the Rust package registry

In addition to these subcommands, Cargo also manages dependencies, compiles and links your code, and handles errors and dependencies automatically. This makes it easier to manage Rust projects and ensures that your application is reliable and efficient. 

## tldr 
 
> Manage Rust projects and their module dependencies (crates).
> Some subcommands such as `cargo build` have their own usage documentation.
> More information: <https://crates.io>.

- Search for crates:

`cargo search {{search_string}}`

- Install a crate:

`cargo install {{crate_name}}`

- List installed crates:

`cargo install --list`

- Create a new binary or library Rust project in the current directory:

`cargo init --{{bin|lib}}`

- Create a new binary or library Rust project in the specified directory:

`cargo new {{path/to/directory}} --{{bin|lib}}`

- Build the Rust project in the current directory:

`cargo build`

- Build the rust project in the current directory using the nightly compiler:

`cargo +nightly build`

- Build using a specific number of threads (default is the number of CPU cores):

`cargo build --jobs {{number_of_threads}}`
