# radare2 
## chatgpt 
`radare2` is a command-line based open-source reverse engineering framework. It is used to analyze and manipulate binary files such as executable programs, libraries, and firmware for various platforms including Linux, macOS, Windows, iOS, and Android. The command `radare2` launches an interactive shell where you can perform various operations on binary files.

Some of the features of `radare2` include:
- Disassembling and decompiling code
- Analyzing binary files for vulnerabilities
- Debugging code
- Patching binary files to modify their behavior
- Scripting and automation capabilities
- Support for multiple architectures and file formats
- Visualizing and graphing code flow and data structures

Radare2 commands are typed in the interactive shell and are similar to Unix commands. Some common commands used in `radare2` are:
- `aaa` - Analyze all binary code, data and strings
- `pdf` - Print disassembly of function
- `VV` - Enter visual mode to display graphs and charts
- `db` - Set breakpoint on a memory address
- `dc` - Continue execution until breakpoint is hit
- `w` - Write changes to the binary file
- `q` - Quit radare2

Overall, `radare2` is a powerful tool for reverse engineering and binary analysis that allows you to gain a deep understanding of how a program works and how to modify its behavior. However, it requires a significant amount of technical knowledge and experience to use effectively. 

## tldr 
 
> A set of reverse engineering tools.
> More information: <https://radare.gitbooks.io/radare2book/>.

- Open a file in write mode without parsing the file format headers:

`radare2 -nw {{path/to/binary}}`

- Debug a program:

`radare2 -d {{path/to/binary}}`

- Run a script before entering the interactive CLI:

`radare2 -i {{path/to/script.r2}} {{path/to/binary}}`

- Show help text for any command in the interactive CLI:

`> {{radare2_command}}?`

- Run a shell command from the interactive CLI:

`> !{{shell_command}}`

- Dump raw bytes of current block to a file:

`> pr > {{path/to/file.bin}}`
