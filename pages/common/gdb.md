# gdb 
## chatgpt 
GDB (GNU Debugger) is a powerful command-line tool used to debug programs written in various programming languages such as C, C++, Objective-C, and others. It allows developers to diagnose and fix errors in programs and provides a variety of features that assist in the debugging process.

The GDB command is used to launch the GDB debugger. When executed, the command opens the GDB shell, where developers can attach or load the compiled program to be debugged. After starting the program, developers can use a range of commands to control the execution of the program, set breakpoints, examine variables, and access memory locations.

The following are some of the many GDB commands that can be used:

- break: Set a breakpoint at a specific line of code or function.
- run: Start the debugging process or continue the execution of the program.
- next: Execute the next line of code.
- step: Execute the next line of code and enter any function calls on that line.
- print: Display the value of a specific variable.
- watch: Monitor a variable and stop the program when the value changes.

Overall, GDB is an essential tool for developers who need to identify and fix errors in their programs during development or testing. 

## tldr 
 
> The GNU Debugger.
> More information: <https://www.gnu.org/software/gdb>.

- Debug an executable:

`gdb {{executable}}`

- Attach a process to gdb:

`gdb -p {{procID}}`

- Debug with a core file:

`gdb -c {{core}} {{executable}}`

- Execute given GDB commands upon start:

`gdb -ex "{{commands}}" {{executable}}`

- Start gdb and pass arguments to the executable:

`gdb --args {{executable}} {{argument1}} {{argument2}}`
