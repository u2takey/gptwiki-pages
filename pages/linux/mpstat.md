# mpstat 
## chatgpt 
The mpstat command is a Linux utility that gives real-time reports about CPU usage in a multi-processor environment. It stands for "multiprocessor statistics" and is used to monitor the utilization of processors, each running parallel processes. When you run the mpstat command, it displays a detailed report on the system's processor usage, giving information about the following:

1. Overall usage percentage: This shows the percentage of CPU utilization across all cores.

2. Individual core statistics: This shows the average usage percentage of each CPU core.

3. Total system statistics: This displays the overall CPU usage, along with other statistics such as system interrupts and context switches.

4. Advanced Processor Statistics: This provides a more in-depth look at the CPU usage like I/O statistics as well.

The mpstat command can help you diagnose performance issues by providing a view of how much CPU power is being used and by what processes. You can also use mpstat to determine if a particular CPU core is overutilized or underutilized, and it can help identify a process that is making excessive demands on the CPU. Overall, the mpstat command is a useful tool for system administrators and developers to monitor and optimize system performance. 

## tldr 
 
> Report CPU statistics.
> More information: <https://manned.org/mpstat>.

- Display CPU statistics every 2 seconds:

`mpstat {{2}}`

- Display 5 reports, one by one, at 2 second intervals:

`mpstat {{2}} {{5}}`

- Display 5 reports, one by one, from a given processor, at 2 second intervals:

`mpstat -P {{0}} {{2}} {{5}}`
