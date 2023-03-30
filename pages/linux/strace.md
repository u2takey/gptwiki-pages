# strace 
## chatgpt 
The `strace` command is a Linux utility that intercepts and records the system calls made by a process. It can be used to diagnose and debug problems with a program by tracing its behavior at a low level.

When you run `strace` followed by a command, it will execute the specified command and print out a detailed log of all system calls made by the process. This includes information about the arguments passed to each system call, its return value, and any errors encountered.

Some common uses of `strace` include:

- Debugging: When a program is misbehaving or crashing, `strace` can be used to trace its system calls and identify where the problem is occurring.
- Performance tuning: `strace` can be used to analyze the performance of a program by measuring the system calls it makes and how long they take to complete.
- Security auditing: `strace` can be used to monitor a program's interactions with the operating system, allowing security analysts to detect potential exploits or vulnerabilities. 

## tldr 
 
> Troubleshooting tool for tracing system calls.
> More information: <https://manned.org/strace>.

- Start tracing a specific process by its PID:

`strace -p {{pid}}`

- Trace a process and filter output by system call:

`strace -p {{pid}} -e {{system_call_name}}`

- Count time, calls, and errors for each system call and report a summary on program exit:

`strace -p {{pid}} -c`

- Show the time spent in every system call:

`strace -p {{pid}} -T`

- Start tracing a program by executing it:

`strace {{program}}`

- Start tracing file operations of a program:

`strace -e trace=file {{program}}`
