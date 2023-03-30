# rustfmt 
## chatgpt 
`rustfmt` is a command line tool for formatting Rust code. It is used to automatically apply consistent and standardized formatting to Rust code files. The tool is designed to follow the official Rust Style Guide and to help maintain consistent code style within a project, among project contributors, and across the Rust community.

The `rustfmt` command works by parsing the source code file or directory, and then automatically applying the formatting rules to the code. The resulting formatted code is then saved to the original file or a new file, depending on the options used.

`rustfmt` supports several configuration options, allowing users to customize the formatting style to their preference. Some of the options include line width, indentation, brace placement, and whitespace usage.

In summary, `rustfmt` is a command line tool that helps developers maintain consistent code formatting and follow the official Rust Style Guide. It is a valuable tool for ensuring that code is easy to read and understand, especially in large codebases. 

## tldr 
 
> Tool for formatting Rust source code.
> More information: <https://github.com/rust-lang/rustfmt>.

- Format a file, overwriting the original file in-place:

`rustfmt {{path/to/source.rs}}`

- Check a file for formatting and display any changes on the console:

`rustfmt --check {{path/to/source.rs}}`

- Backup any modified files before formatting (the original file is renamed with a `.bk` extension):

`rustfmt --backup {{path/to/source.rs}}`
