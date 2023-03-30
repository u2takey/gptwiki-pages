# cargo add 
## chatgpt 
"Cargo add" is a command used in Rust programming language and the Cargo package manager. It is used to add a new dependency to a Rust project.

When you run the "cargo add" command, you need to specify two things: the name of the dependency you want to add and the version you want to use. For example, if you want to add the "serde" dependency to your project, you would run the following command:

```
cargo add serde --version 1.0.104
```

This command will add the "serde" dependency to your project and specify that version 1.0.104 should be used.

"Cargo add" not only installs the specified dependency but also updates your Cargo.toml file with the new dependency and its version. Cargo creates a new section in the `Cargo.toml` file as `[dependencies.<package_name>]` for each dependency, where `<package_name>` is the name of the dependency you specified.

For example, after running the above command, the `[dependencies]` section in the `Cargo.toml` file will look like:

```
[dependencies]
serde = "1.0.104"
```

This way, when you want to build or run your Rust program, Cargo will know what dependencies are required and automatically download and build them.

Overall, "cargo add" is a very useful command for managing dependencies in Rust projects, as it simplifies the process of adding, updating, and removing dependencies. 

## tldr 
 
> Add dependencies to a Rust project's `Cargo.toml` file.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-add.html>.

- Add the latest version of a dependency to the current project:

`cargo add {{dependency}}`

- Add a specific version of a dependency:

`cargo add {{dependency}}@{{version}}`

- Add a dependency and enable one or more specific features:

`cargo add {{dependency}} --features {{feature_1}},{{feature_2}}`

- Add an optional dependency, which then gets exposed as a feature of the crate:

`cargo add {{dependency}} --optional`

- Add a local crate as a dependency:

`cargo add --path {{path/to/crate}}`

- Add a development or build dependency:

`cargo add {{dependency}} --{{dev|build}}`

- Add a dependency with all default features disabled:

`cargo add {{dependency}} --no-default-features`
