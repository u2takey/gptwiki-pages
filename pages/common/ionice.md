# ionice 
## chatgpt 
The `ionice` command is used to set or get the I/O scheduling class and priority for a program. I/O stands for Input/Output, and it refers to the access and manipulation of data between a program and a storage device such as a hard disk or SSD. 

I/O operations can be resource-intensive and may impact system performance, especially when multiple programs are running simultaneously. The `ionice` command allows us to control the I/O priority of a program to prioritize or limit its access to the storage device.

The `ionice` command can be used in combination with the `nice` command, which sets the CPU scheduling priority for a program.

Syntax:
```
ionice [-c CLASS] [-n LEVEL] [-t PID | COMMAND [ARG]...]
```

Options:
- `-c CLASS`: Specifies the I/O scheduling class for the program. There are three classes available:
  - `0`: none - no I/O scheduling priority is set (default)
  - `1`: real-time - high-priority I/O operations
  - `2`: best-effort - normal I/O priority
  - `3`: idle - low-priority I/O operations
- `-n LEVEL`: Specifies the I/O scheduling priority for the program. The priority level ranges from 0 to 7, where 0 is the highest priority and 7 is the lowest priority. The default value is 4.
- `-t PID`: Specifies the process ID of the program to change I/O priority for.
- `COMMAND [ARG]...`: Specifies the command and its arguments to run with a specific I/O priority.

Examples:
1. To set the I/O priority of a program with a specific PID:
```
ionice -c 3 -n 0 -t 1234
```
This command changes the I/O scheduling class to idle and the priority level to the highest for the program with the PID 1234.

2. To run a command with a specific I/O priority:
```
ionice -c 2 -n 4 dd if=/dev/zero of=/dev/null bs=1M count=100
```
This command runs the `dd` command with I/O scheduling class set to best-effort and priority level set to 4 (default), while copying 100 MB of data from `/dev/zero` to `/dev/null`.

Note: The `ionice` command requires root privileges to run. 

## tldr 
 
> Get or set program I/O scheduling class and priority.
> Scheduling classes: 1 (realtime), 2 (best-effort), 3 (idle).
> Priority levels: 0 (the highest) - 7 (the lowest).
> More information: <https://manned.org/ionice>.

- Set I/O scheduling class of a running process:

`ionice -c {{scheduling_class}} -p {{pid}}`

- Run a command with custom I/O scheduling class and priority:

`ionice -c {{scheduling_class}} -n {{priority}} {{command}}`

- Print the I/O scheduling class and priority of a running process:

`ionice -p {{pid}}`
