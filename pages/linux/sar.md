# sar 
## chatgpt 
The `sar` command is a system monitoring and reporting tool that is used to analyze and report system resource usage, such as CPU, memory, disk I/O, and network I/O activity on Linux and Unix-based operating systems. It is short for "System Activity Reporter". 

The tool reads the system data collected by the kernel, and displays the usage statistics in various formats, including tables, graphs, and raw data. The command takes various parameters to specify the type of information to be displayed, the interval time, and the number of iterations.

Here are some of the commonly used parameters with the `sar` command:

- `-u`: reports CPU utilization metrics such as user time, system time, idle time, etc.
- `-r`: reports memory utilization metrics such as free memory, used memory, and swap space.
- `-d`: reports disk I/O metrics such as disk read/write rates, disk utilization, etc.
- `-n`: reports network I/O metrics such as TCP/UDP throughput, packet loss, etc.
- `-f`: specifies the input file to read the data from.
- `-h`: prints the help message for the command.
- `-V`: prints the version of the `sar` command.

For example, to check the CPU utilization every 5 seconds, you can use the command:

`sar -u 5`

This will display a real-time report of CPU usage with a five-second interval. You can use the Ctrl+C key combination to stop the report.

In summary, the `sar` command is a versatile tool that provides a detailed analysis of the system resource usage, which can be useful in troubleshooting performance issues and identifying resource-intensive processes. 

## tldr 
 
> Monitor performance of various Linux subsystems.
> More information: <https://manned.org/sar>.

- Report I/O and transfer rate issued to physical devices, one per second (press CTRL+C to quit):

`sar -b {{1}}`

- Report a total of 10 network device statistics, one per 2 seconds:

`sar -n DEV {{2}} {{10}}`

- Report CPU utilization, one per 2 seconds:

`sar -u ALL {{2}}`

- Report a total of 20 memory utilization statistics, one per second:

`sar -r ALL {{1}} {{20}}`

- Report the run queue length and load averages, one per second:

`sar -q {{1}}`

- Report paging statistics, one per 5 seconds:

`sar -B {{5}}`
