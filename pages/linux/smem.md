# smem 
## chatgpt 
The smem command stands for "memory usage by process in Linux". It is used to display the memory usage of individual processes and system memory usage in Linux. 

When run without any options or arguments, smem displays a summary of the memory usage broken down by several categories, including the total system memory usage, the usage of kernel memory, shared memory, and individual processes.

smem can also be used to display memory usage for a specific process or group of processes. For example, to display memory usage for a process with a specific PID (process ID), you can run:

smem -p PID

This command will display the memory usage for the process with the given PID.

You can also use smem to display memory usage for a group of processes, such as all processes owned by a specific user. For example, to display memory usage for all processes owned by the user "user1", you can run:

smem -u user1

This command will display the memory usage for all processes owned by the user "user1".

Overall, smem is a useful command for monitoring memory usage in Linux, and can help identify memory usage patterns and potential memory-related issues. 

## tldr 
 
> Print memory usage for programs.
> More information: <https://manned.org/smem>.

- Print memory usage for current processes:

`smem`

- Print memory usage for current processes for a every user on a system:

`smem --users`

- Print memory usage for current processes for a specified user:

`smem --userfilter {{username}}`

- Print system memory information:

`smem --system`
