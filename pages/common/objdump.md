# objdump 
## chatgpt 
Objdump is a command-line utility that allows users to examine and analyze object files in various formats. The utility can be used to disassemble executables, dump section headers and contents, symbol tables, relocation tables, and other useful information.

The basic syntax for using objdump is as follows:

`objdump [options] [[section | filename]...]`

The options that can be used with the objdump command are numerous, but some commonly used ones include:

- `-d`: disassemble the binary code and print assembly instructions
- `-s`: dump the contents of a given section
- `-t`: print the symbol table
- `-r`: print the relocation information
- `-x`: print all header information

The section or filename argument specifies the section or file to analyze with objdump. If no argument is provided, objdump will default to displaying all sections and symbols in the provided file.

Overall, objdump is a powerful tool for analyzing and understanding the contents of object files, and can be useful for developers and security professionals alike. 

## tldr 
 
> View information about object files.
> More information: <https://manned.org/objdump>.

- Display the file header information:

`objdump -f {{binary}}`

- Display the disassembled output of executable sections:

`objdump -d {{binary}}`

- Display the disassembled executable sections in intel syntax:

`objdump -M intel -d {{binary}}`

- Display a complete binary hex dump of all sections:

`objdump -s {{binary}}`
