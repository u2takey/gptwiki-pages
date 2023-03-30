# cargo test 
## chatgpt 
The `cargo test` command is used in Rust programming language to execute the unit tests defined in a Rust project.

When the `cargo test` command is executed, Rust's build system automatically builds the project and runs all the tests that are defined within the project. The test results are then displayed on the command-line interface.

Some of the things that the `cargo test` command does include:

- Compiling the project's source code along with its test code
- Running all the tests defined in the project
- Capturing and displaying the test output and results
- Collecting and displaying coverage data, if enabled

The `cargo test` command has several options that can be used to customize its behavior, including:

- `--release`: Run tests in release mode rather than debug mode
- `-- --test-threads=NUM`: Specify the number of test threads to run simultaneously (the default is to use as many threads as there are available logical CPUs)
- `-- --ignored`: Run only the tests that are marked with the `#[ignore]` attribute
- `--no-fail-fast`: Run all tests even if some fail (the default is to stop running tests as soon as a failure occurs)

Overall, the `cargo test` command is an essential tool for Rust developers to ensure their code is functioning correctly and to catch any errors or bugs. 

## tldr 
 
> Execute the unit and integration tests of a Rust package.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-test.html>.

- Only run tests containing a specific string in their names:

`cargo test {{testname}}`

- Set the number of simultaneous running test cases:

`cargo test -- --test-threads={{count}}`

- Require that `Cargo.lock` is up to date:

`cargo test --locked`

- Test artifacts in release mode, with optimizations:

`cargo test --release`

- Test all packages in the workspace:

`cargo test --workspace`

- Run tests for a package:

`cargo test --package {{package}}`

- Run tests without hiding output from test executions:

`cargo test -- --nocapture`
