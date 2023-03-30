# wasm-objdump 
## chatgpt 
`wasm-objdump` is a command-line tool that is used to disassemble a WebAssembly binary file. It provides a human-readable representation of the binary file's contents, allowing developers to examine the structure and instructions of the WebAssembly module. The tool reads a binary file and outputs a textual representation of the binary file's contents, including the function signatures, import and export definitions, memory layouts, and code segments. 

The `wasm-objdump` command takes the following arguments:

- `-h/--help`: This argument displays the help message and exits.
- `-x/--headers`: This argument prints the headers of the WebAssembly file, such as the Magic Number, version, and section information.
- `-s/--sections`: This argument lists all of the sections within the WebAssembly file.
- `-d/--disassemble`: This argument disassembles the code segments of the WebAssembly module and prints the corresponding WebAssembly instructions.
- `-D/--disassemble-all`: This argument disassembles all of the sections of the WebAssembly file, including the data segments and custom sections.
- `-r/--reloc`: This argument displays the relocations of the WebAssembly file.

In summary, `wasm-objdump` is a command-line tool used to disassemble a WebAssembly binary file, providing a human-readable representation of its contents for analysis and debugging purposes. 

## tldr 
 
> Display information from WebAssembly binaries.
> More information: <https://github.com/WebAssembly/wabt>.

- Display the section headers of a given binary:

`wasm-objdump -h {{file.wasm}}`

- Display the entire disassembled output of a given binary:

`wasm-objdump -d {{file.wasm}}`

- Display the details of each section:

`wasm-objdump --details {{file.wasm}}`

- Display the details of a given section:

`wasm-objdump --section '{{import}}' --details {{file.wasm}}`
