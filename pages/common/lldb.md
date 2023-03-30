# lldb 
## chatgpt 
`lldb` is a command-line debugger for macOS, used for debugging programs written in C, C++, Objective-C, and Swift. It provides features such as source-level debugging, console-like command interface, support for multiple CPU architectures, and remote debugging capabilities.

Here are some basic commands and their descriptions:

- `lldb <program>`: starts `lldb` and loads the executable `program`. You can add command-line arguments after `program`.
- `breakpoint set`: sets a breakpoint at a specified line or function in the source code.
- `run`: runs the program until it hits a breakpoint or terminates.
- `next`: executes the next line of source code in the current function context.
- `step`: executes the next line of source code, but if the line contains a function call, it will stop at the first line of the function and allow you to step inside it.
- `continue`: resumes execution after it stopped at a breakpoint.
- `print <expression>`: evaluates the given `expression` and prints its value.
- `watchpoint set`: sets a watchpoint at a specified variable or memory address. The program stops when the value at that location changes.
- `quit`: exits the debugger.

For more advanced usage, `lldb` offers many more commands and options. You can refer to the official documentation for more information. 

## tldr 
 
> The LLVM Low-Level Debugger.
> More information: <https://lldb.llvm.org>.

- Debug an executable:

`lldb {{executable}}`

- Attach `lldb` to a running process with a given PID:

`lldb -p {{pid}}`

- Wait for a new process to launch with a given name, and attach to it:

`lldb -w -n {{process_name}}`
