# wasm2c 
## chatgpt 
wasm2c is a command-line tool that converts WebAssembly (WASM) code into C code. The generated C code can then be compiled into native code for execution on platforms that support C.

The command is typically used in the following format:

```
wasm2c [OPTIONS] input.wasm -o output.c
```

where:

- `input.wasm`: the input WASM file to be converted to C code
- `-o`: an option to specify the output file
- `output.c`: the output C file where the generated code is saved.

Some of the options available with wasm2c include:

- `-v`: print version information
- `-h`: print help
- `--pedantic`: strict error checking
- `--bulk-memory`: enable proposals for bulk memory operations
- `--debug-parser`: output parser debug information
- `--debug-names`: print debug names
- `--no-output`: disable file output

The converted C code can be modified and optimized before it is compiled into native code using a C compiler. WASM code is often used for portable code execution and is supported by many web browsers and other platforms. Converting it to C code using wasm2c can make it easier to use on systems that do not support WASM natively. 

## tldr 
 
> Convert a file from the WebAssembly binary format to a C source file and header.
> More information: <https://github.com/WebAssembly/wabt>.

- Convert a file to a C source file and header and display it to the console:

`wasm2c {{file.wasm}}`

- Write the output to a given file (`file.h` gets additionally generated):

`wasm2c {{file.wasm}} -o {{file.c}}`
