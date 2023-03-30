# cargo doc 
## chatgpt 
The "cargo doc" command is a command-line tool used in Rust programming language, specifically for generating documentation for a Rust package. When you run "cargo doc" in the terminal, Rust's package manager "Cargo" looks for documentation comments (also known as "doc comments") written in the source code files of the package, and generates HTML files to document the package.

More specifically, "cargo doc" performs the following steps:

1. It parses the package's source code files, looking for Rustdoc comments.

2. It runs Rust's built-in documentation generator, Rustdoc, which creates HTML files that document the package's APIs, structs, functions, and modules.

3. It puts the generated HTML files in the "target/doc" directory of the package.

By default, "cargo doc" generates documentation only for the current package, but you can pass additional options to the command to generate documentation for all packages in the current workspace or for external packages.

The generated documentation includes:

- Rustdoc comments for each item (e.g., functions, structs, enums) in the source code

- Usage examples for each item

- A summary of the module hierarchy

- A list of crates that the package depends on

The generated documentation can be published to a public or private website, hosted on a local or remote server, or shared as a file or a ZIP archive. The documentation website can be styled and customized using CSS and JavaScript.

Overall, "cargo doc" is an essential tool for Rust developers, as it makes it easy to document and share their code with other developers. It enables developers to create comprehensive and up-to-date documentation that helps users of their packages understand how to use them, which functions are available, and how they work. 

## tldr 
 
> Build and view Rust package documentation offline.
> More information: <https://doc.rust-lang.org/cargo/commands/cargo-doc.html>.

- Build and view the default package documentation in the browser:

`cargo doc --open`

- Build documentation without accessing the network:

`cargo doc --offline`

- View a particular package's documentation:

`cargo doc --open --package {{package}}`

- View a particular package's documentation offline:

`cargo doc --open --offline --package {{package}}`
