# nm 
## chatgpt 
The "nm" command is a Unix/Linux utility that is used to display the symbol table of an object file, archive library, or an executable. The symbol table contains information about the symbols or objects defined or referenced in the program, such as function names, variable names, and their addresses or types.

The syntax of the "nm" command is:
```
nm [options] [files]
```

The "files" argument specifies the object files or libraries to be examined. Multiple files can be specified, separated by spaces.

Some common options of the "nm" command are as follows:
- -g: Display only global (external) symbols.
- -D: Display only dynamic symbols.
- -r: Display symbols in reverse order.
- -u: Display undefined symbols.
- -A: Display with BSD-style symbol table.

When executed without any options, the "nm" command displays the symbol table of an object file in hexadecimal format, showing the symbol's value, type, and name. The symbol type is indicated by a single character at the beginning of each line, as follows:
- "U": Undefined symbol
- "T": Text (executable code)
- "D": Data (initialized data)
- "B": BSS (uninitialized data)
- "W": Weak symbol
- "V": Global variable
- "f": Function
- "a": Absolute symbol
- "p": Stack protector symbol

The "nm" command is often used in conjunction with other Unix/Linux utilities, such as "grep", "awk", and "sort", to extract specific information from the symbol table or to compare symbol tables of different versions of a program. 

## tldr 
 
> List symbol names in object files.
> More information: <https://manned.org/nm>.

- List global (extern) functions in a file (prefixed with T):

`nm -g {{path/to/file.o}}`

- List only undefined symbols in a file:

`nm -u {{path/to/file.o}}`

- List all symbols, even debugging symbols:

`nm -a {{path/to/file.o}}`

- Demangle C++ symbols (make them readable):

`nm --demangle {{path/to/file.o}}`
