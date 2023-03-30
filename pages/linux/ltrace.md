# ltrace 
## chatgpt 
The 'ltrace' command is a Linux tool that is used for debugging and tracing dynamic library calls made by a running process. When an application or a process is executed, it may use libraries that are not present in its binary file. These libraries are loaded dynamically into memory during the runtime, and their functions are called using dynamic linking. The 'ltrace' command can be used to intercept these library calls and display information about them.

The syntax of the 'ltrace' command is as follows:

```
ltrace [OPTIONS] [COMMAND [ARGUMENTS]]
```

The 'ltrace' command has several options that can be used to customize its behavior. Some of the widely used options are:

- -f: Traces all child processes of the specified command.
- -c: Displays a summary of the number of times each function was called.
- -s: Limits the length of the string that is displayed for each function call.
- -t: Shows the time taken by each function call.

Once the 'ltrace' command is executed with appropriate options, it will start tracing the library calls made by the specified command. It will print information on the screen about function calls such as function names, return values, and parameter values.

For example, if we wanted to trace the standard 'ls' command and display the library calls it makes, we could execute the following command:

```
ltrace ls
```

This will display the list of library calls made by the 'ls' command, along with their respective parameters and return values. By analyzing this information, we can gain insights into the behavior of the command and identify any errors or performance issues. 

## tldr 
 
> Display dynamic library calls of a process.
> More information: <https://manned.org/ltrace>.

- Print (trace) library calls of a program binary:

`ltrace ./{{program}}`

- Count library calls. Print a handy summary at the bottom:

`ltrace -c {{path/to/program}}`

- Trace calls to malloc and free, omit those done by libc:

`ltrace -e malloc+free-@libc.so* {{path/to/program}}`

- Write to file instead of terminal:

`ltrace -o {{file}} {{path/to/program}}`
