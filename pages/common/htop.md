# htop 
## chatgpt 
`htop` is a command-line utility for Linux and Unix-based operating systems which allows users to monitor the system's CPU and memory usage, as well as view detailed information about running processes. The utility provides a real-time view of the system's performance and displays the following details:

- Load average: The load average is the average number of processes in a run queue over a particular period of time. It represents the system's workload and indicates how busy the system is.

- CPU usage: This shows the percentage of CPU being used by processes on the system. The CPU usage bar for each process is color-coded, with red indicating a process that is using more than 75% of the CPU, yellow indicating a process that is using between 50% and 75% of the CPU, and green indicating a process that is using less than 50% of the CPU.

- Memory usage: This shows the amount of memory being used by processes on the system. The memory usage bar for each process is color-coded, with red indicating a process that is using more than 75% of the available memory, yellow indicating a process that is using between 50% and 75% of the memory, and green indicating a process that is using less than 50% of the memory.

- Processes: This shows a list of all running processes on the system. Each process is listed with its name, process ID (PID), user, CPU usage, memory usage, and other information.

- Command-line arguments: This shows the command-line arguments used to start each process.

- Thread count: This shows the number of threads being used by each process.

- Priority: This shows the priority of each process.

htop also allows users to manage running processes by providing options to kill, renice, or pause a process. It is a powerful system monitoring tool that can help identify resource-hungry processes and optimize system performance. 

## tldr 
 
> Display dynamic real-time information about running processes. An enhanced version of `top`.
> More information: <https://htop.dev/>.

- Start htop:

`htop`

- Start htop displaying processes owned by a specific user:

`htop --user {{username}}`

- Sort processes by a specified `sort_item` (use `htop --sort help` for available options):

`htop --sort {{sort_item}}`

- See interactive commands while running htop:

`?`

- Switch to a different tab:

`tab`

- Display help:

`htop --help`
