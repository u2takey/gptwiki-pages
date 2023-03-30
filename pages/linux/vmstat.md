# vmstat 
## chatgpt 
The `vmstat` command is a Linux utility that provides a system-level view of the current virtual memory statistics including CPU usage, memory utilization, i/o statistics, and process activity. The output is displayed in the form of a table that is updated at a specified interval.

The columns produced by `vmstat` are as follows:

1. Procs - displays the number of processes in different states such as running, blocked, and waiting for I/O.

2. Memory - displays the current memory usage of the system in Kilobytes (KB). This includes fields such as Swap, Free, Buffers, and Cached.

3. Swap - displays the current status of swap space in the system. Swap space is used to extend RAM and provide additional memory when required. 

4. IO - provides a snapshot of the Input and Output operations of the system. Fields include bi (blocks received from a block device), bo (blocks sent to a block device), and bi8 (blocks received from a block device in 8KB units - this field is only available on newer kernel versions.)

5. System - provides CPU statistics, including the percentage of time that the system has spent in user space or kernel space.

6. CPU - displays the system's CPU statistics. This includes fields such as us (user time), sy (system time), id (idle time), wa (time spent on waiting for I/O), and st (time stolen from a virtual machine).

Overall, `vmstat` is an effective tool for investigating and monitoring system performance issues on a Linux system. 

## tldr 
 
> Report information about processes, memory, paging, block IO, traps, disks and CPU activity.
> More information: <https://manned.org/vmstat>.

- Display virtual memory statistics:

`vmstat`

- Display reports every 2 seconds for 5 times:

`vmstat {{2}} {{5}}`
