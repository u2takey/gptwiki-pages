# rabin2 
## chatgpt 
`rabin2` is a command-line tool that is part of the Radare2 reverse engineering framework. This tool is used to analyze various aspects of binary files, including executable files, libraries, and object files. The `rabin2` command has several subcommands that allow users to perform different types of analysis on a target binary file. Here are some of the most commonly used subcommands of `rabin2`:

- `info`: This subcommand is used to display general information about the binary file, such as its entry point, file format, architecture, sections, and symbols.
- `sections`: This subcommand is used to list the sections present in the binary file, along with their addresses, sizes, and flags.
- `symbols`: This subcommand is used to list the symbols (functions, variables, etc.) present in the binary file, along with their addresses and types.
- `imports`: This subcommand is used to list the imported functions and their addresses.
- `exports`: This subcommand is used to list the exported functions and their addresses.
- `strings`: This subcommand is used to list the ASCII and Unicode strings present in the binary file.
- `hash`: This subcommand is used to calculate various hash values (MD5, SHA1, SHA256, etc.) for the binary file.
- `entrypoint`: This subcommand is used to display the address of the entry point of the binary file.
- `size`: This subcommand is used to display the size of the binary file.

These are just some examples of the subcommands that `rabin2` offers. Users can consult the tool's documentation for a full list of available subcommands and their respective parameters. 

## tldr 
 
> Get information about binary files (ELF, PE, Java CLASS, Mach-O) - symbols, sections, linked libraries, etc.
> Comes bundled with `radare2`.
> More information: <https://manned.org/rabin2>.

- Display general information about a binary (architecture, type, endianness):

`rabin2 -I {{path/to/binary}}`

- Display linked libraries:

`rabin2 -l {{path/to/binary}}`

- Display symbols imported from libraries:

`rabin2 -i {{path/to/binary}}`

- Display strings contained in the binary:

`rabin2 -z {{path/to/binary}}`

- Display the output in JSON:

`rabin2 -j -I {{path/to/binary}}`
