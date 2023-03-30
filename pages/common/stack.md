# stack 
## chatgpt 
As an AI language model, I assume you are referring to the `stack` command in Linux/Unix operating systems. 

The `stack` command is used to display the stack trace of a running process. A stack trace is a list of function calls that are currently being executed by the program, along with their parameters and the line numbers where they are called from. The stack trace is usually used to diagnose and debug issues in the program, especially when it crashes.

Here is the syntax of the `stack` command:

```
stack [options] <pid>
```

- `options`: Additional command-line options that can be used to customize the output of the command.
- `<pid>`: The process ID of the program whose stack trace is to be displayed.

The `stack` command is usually used in combination with other debugging tools like `gdb` to analyze the program's behavior and isolate the cause of the issues. Some of the commonly used options of the `stack` command are:

- `-p`: Prints only the function names, without showing the line numbers and parameters.
- `-H`: Highlight the current function in the trace with an asterisk.
- `-f`: Prints the full path of the source file where the function is defined.
- `-o`: Prints the offset of the function call from the start of the program code.

It's important to note that the `stack` command requires root privileges to be able to display the stack trace of processes that don't belong to the current user. 

## tldr 
 
> Tool for managing Haskell projects.
> More information: <https://github.com/commercialhaskell/stack>.

- Create a new package:

`stack new {{package_name}} {{template_name}}`

- Compile a package:

`stack build`

- Run tests inside a package:

`stack test`

- Compile a project and re-compile every time a file changes:

`stack build --file-watch`

- Compile a project and execute a command after compilation:

`stack build --exec "{{command}}"`

- Run a program and pass an argument to it:

`stack exec {{program_name}} -- {{argument}}`
