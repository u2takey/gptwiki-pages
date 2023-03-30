# nasm 
## chatgpt 
nasm is a command that stands for "Netwide Assembler". It is a command-line utility that allows developers to compile assembly code into executable machine code for different processors and operating systems. 

The syntax for using the nasm command is:

nasm [options] [filename]

Options are settings that can be customized to fit specific needs. Some of the commonly used options are:

- -f: sets the output format for the executable (e.g., -f elf for Linux, -f win32 for Windows)
- -g: includes debugging information in the output file
- -o: specifies the name and path of the output file
- -w: specifies warning levels (e.g., -w-all for all warnings)

[filename] is the name and path of the assembly code file to be compiled.

For example, to compile an assembly code file named "hello.asm" to run on Linux in the ELF format, the command would be:

nasm -f elf hello.asm

This would generate an executable file named "hello" in the same directory as "hello.asm". The resulting executable can be executed using "./hello" in the Linux terminal. 

## tldr 
 
> The Netwide Assembler, a portable 80x86 assembler.
> More information: <https://nasm.us>.

- Assemble `source.asm` into a binary file `source`, in the (default) raw binary format:

`nasm {{source.asm}}`

- Assemble `source.asm` into a binary file `output_file`, in the specified format:

`nasm -f {{format}} {{source.asm}} -o {{output_file}}`

- List valid output formats (along with basic nasm help):

`nasm -hf`

- Assemble and generate an assembly listing file:

`nasm -l {{list_file}} {{source.asm}}`

- Add a directory (must be written with trailing slash) to the include file search path before assembling:

`nasm -i {{path/to/include_dir/}} {{source.asm}}`
