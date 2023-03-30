# free 
## chatgpt 
The `free` command is a Linux utility that provides information about the system memory usage. When you enter the command `free` in the terminal, the output displays the amount of free and used memory in the system, including the total amount of physical memory, the amount of memory used by the operating system and processes, the amount of memory currently free, the amount of memory used for disk buffers and cache, and the total amount of swap space available and used.

The output of the `free` command consists of the following columns:

- `total`: Total amount of physical memory available in the system.
- `used`: Amount of memory used by the operating system, kernel, and all the running processes.
- `free`: Amount of memory currently not being used by any process or kernel buffers.
- `shared`: Amount of shared memory used by the system.
- `buff/cache`: Amount of memory used for disk buffer and cache.
- `available`: Amount of memory that is immediately available to the system without any additional swap usage.

The memory values are displayed in either kilobytes (KB), megabytes (MB), or gigabytes (GB), depending on the memory size of the system. The `free` command is a useful tool for checking the system’s memory usage and identifying any potential memory issues or constraints. 

## tldr 
 
> Display amount of free and used memory in the system.
> More information: <https://manned.org/free>.

- Display system memory:

`free`

- Display memory in Bytes/KB/MB/GB:

`free -{{b|k|m|g}}`

- Display memory in human-readable units:

`free -h`

- Refresh the output every 2 seconds:

`free -s {{2}}`
