# runlim 
## chatgpt 
The runlim command is a utility provided by the LimTime package for limiting the resource usage of a process. This command sets resource limits, such as limiting the amount of CPU time available to a process, the amount of memory that the process can allocate, the maximum number of open files, the number of processes a user can spawn, and several other resources.

The syntax of the runlim command is as follows:

runlim [-t <time_limit>] [-v <virtual_memory_limit>] 
[-h <heap_memory_limit>] [<command> [<argument> ...]]

Here are the explanations of the various options:

- `-t <time_limit>` - sets the time limit for CPU time usage in seconds.
- `-v <virtual_memory_limit>` - sets the Virtual Memory (VM) limit in bytes.
- `-h <heap_memory_limit>` - sets the heap memory limit in bytes.
- `<command>` - specifies the command or script to be executed.
- `<argument>` - specifies the command line arguments to be passed to the command.

For example, to limit the CPU time usage of a command to 10 seconds, you can use the following command:

`runlim -t 10 <command>`

This command runs the process specified by <command>, and if it exceeds the specified CPU time limit, it will be terminated.

Similarly, to limit the maximum amount of virtual memory allocated by a command to 1 GB, you can use the following command:

`runlim -v 1000000000 <command>`

Note that the exact syntax and available options may differ based on the version and distribution of the LimTime package. 

## tldr 
 
> A tool for sampling and limiting time and memory usage of a program and its child processes using the proc file system on Linux.
> More information: <http://fmv.jku.at/runlim>.

- Print the time and memory usage of a command:

`runlim {{command}} {{command_arguments}}`

- Log statistics to a file instead of `stdout`:

`runlim --output-file={{path/to/file}} {{command}} {{command_arguments}}`

- Limit time to an upper bound (in seconds):

`runlim --time-limit={{number}} {{command}} {{command_arguments}}`

- Limit real-time to an upper bound (in seconds):

`runlim --real-time-limit={{number}} {{command}} {{command_arguments}}`

- Limit space to an upper bound (in MB):

`runlim --space-limit={{number}} {{command}} {{command_arguments}}`
