# prlimit 
## chatgpt 
prlimit is a Linux command-line utility that allows a user to view and modify the resource limits of a running process. Resource limits specify the maximum amount of CPU time, memory, file descriptors, and other system resources that a process can consume. 

The syntax of the prlimit command is as follows:

`prlimit [options] pid`

where "pid" is the process ID of the target process, and "options" are the command-line options used to specify the resource limit to be set, queried, or modified.

The most commonly used options of the prlimit command are as follows:

- `-p, --pid`: specifies the process ID of the target process.
- `-v, --data`: sets or queries the maximum data segment size (in bytes).
- `-c, --core`: sets or queries the maximum size of core dumps.
- `-f, --files`: sets or queries the maximum number of open file descriptors.
- `-n, --nofile`: sets or queries the maximum number of open file descriptors for a specific file type.
- `-t, --cpu`: sets or queries the maximum CPU time (in seconds) that a process may use.
- `-m, --memlock`: sets or queries the maximum amount of memory that may be locked into RAM.
- `-i, --sigpending`: sets or queries the maximum number of pending signals.
- `-q, --msgqueue`: sets or queries the maximum size of POSIX message queues.
- `-r, --rss`: sets or queries the maximum resident set size (in bytes).
- `-s, --stack`: sets or queries the maximum stack segment size (in bytes).

By default, the prlimit command prints the existing resource limits of the specified process. However, by using the appropriate options, a user can modify the limits as well.

For example, to set the maximum number of open files for a specific process with PID 1234 to 1000, the following command can be used:

`prlimit -n1000 -p1234`

This will limit the number of open file descriptors for the process to 1000. Similarly, the other resource limits can be set or queried using the appropriate options. 

## tldr 
 
> Get or set process resource soft and hard limits.
> Given a process ID and one or more resources, prlimit tries to retrieve and/or modify the limits.
> More information: <https://manned.org/prlimit>.

- Display limit values for all current resources for the running parent process:

`prlimit`

- Display limit values for all current resources of a specified process:

`prlimit --pid {{pid number}}`

- Run a command with a custom number of open files limit:

`prlimit --nofile={{10}} {{command}}`
