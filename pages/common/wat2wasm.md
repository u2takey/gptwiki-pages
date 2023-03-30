# wat2wasm 
## chatgpt 
wat2wasm is a command-line tool that is used to convert WebAssembly text format (known as WebAssembly textual representation or simply WAT) to WebAssembly binary format (known as WebAssembly binary representation or simply WASM).

WebAssembly text format (WAT) is a human-readable representation of WebAssembly bytecode. It is used to write WebAssembly modules in a more human-readable and writable way, making it easier to read, write, and debug. It uses a syntax that is similar to JavaScript and allows developers to express complex logic in a concise manner.

However, while WAT is human-readable, it is not directly executable by the browser or runtime environment. It needs to be translated into WebAssembly binary format or WASM, which is a compact binary format that is designed to be fast to load, execute, and validate.

This is where wat2wasm comes into play. It is a command that takes a WAT file as input and converts it into a WASM file that can be executed by WebAssembly-compatible environments. The syntax for using wat2wasm is simple:

```
wat2wasm [options] input.wat -o output.wasm
```

Where "input.wat" is the input WAT file, "output.wasm" is the output WASM file, and "[options]" are the various options that can be used to control the conversion process.

The options include things like:

- --help: Shows a help message with all the available options
- --enable-exceptions: Enables the use of exceptions for easier error handling in the generated WASM code
- --inline-imports: Inlines function imports for better performance
- --no-check: Disables checks for undefined functions, types, and imports during compilation

Once the command is executed successfully, the output file can be used just like any other WASM file, and can be loaded into a runtime environment using tools like webassembly.js, wasm-pack, or any other WebAssembly-compatible runtime. 

## tldr 
 
> Convert a file from the WebAssembly text format to the binary format.
> More information: <https://github.com/WebAssembly/wabt>.

- Parse and check a file for errors:

`wat2wasm {{file.wat}}`

- Write the output binary to a given file:

`wat2wasm {{file.wat}} -o {{file.wasm}}`

- Display simplified representation of every byte:

`wat2wasm -v {{file.wat}}`
