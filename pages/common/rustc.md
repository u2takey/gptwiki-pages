# rustc 
## chatgpt 
Rustc is the command used to compile Rust code. A compiler is a computer program that translates code written in one language (in this case, Rust) into code that can be executed by a computer.

When you run the rustc command followed by the name of a Rust source file, rustc will read the code in the file, check it for errors and then translate it into machine code that can be executed by the computer's processor.

Rustc is a command line tool, so it is typically run from the terminal or command prompt. The basic syntax for using rustc is:

rustc [options] <input file>

The input file is the name of the Rust source file you want to compile. The options are various configuration settings that you can pass to the compiler to control its behavior.

Some common options include:

- --crate-type: Specifies the type of output the compiler should produce (e.g. executable or library)
- --out-dir: Specifies the directory where the compiled code should be written to
- --emit: Specifies the type of output file(s) the compiler should produce (e.g. object files, LLVM IR files, etc.)
- --verbose: Enables verbose output that provides more detailed information about the compiling process.

Once the code has been compiled, you can execute it by running the resulting executable file (if you compiled a standalone program) or by linking to the compiled library if you created a library. 

## tldr 
 
> The Rust compiler.
> Processes, compiles and links Rust language source files.
> More information: <https://doc.rust-lang.org/rustc>.

- Compile a single file:

`rustc {{path/to/file.rs}}`

- Compile with high optimization:

`rustc -O {{path/to/file.rs}}`

- Compile with debugging information:

`rustc -g {{path/to/file.rs}}`

- Compile with architecture-specific optimizations for the current CPU:

`rustc -C target-cpu=native {{path/to/file.rs}}`

- Display architecture-specific optimizations for the current CPU:

`rustc -C target-cpu=native --print cfg`

- Display target list:

`rustc --print target-list`

- Compile for a specific target:

`rustc --target {{target_triple}} {{path/to/file.rs}}`
