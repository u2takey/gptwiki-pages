# dstat 
## chatgpt 
The "dstat" is a Linux command that is used to display system resource statistics in real-time. It provides information on CPU usage, disk activity, network traffic, memory usage, and system load on the machine. 

When run, the “dstat” command will output a table of real-time statistics for each of the resources being monitored. This table will show different columns containing information about different system resources such as CPU usage, disk activity, network traffic and memory usage amongst others. 

The columns in the output table will vary depending on the options and arguments used when running the command. The default output of the command will show a set of columns that include the following:

- CPU usage: This column shows the percentage of the CPU that is currently in use. 
- Disk Activity: This column shows the read and write speed of the different disks attached to the system.
- Network: This column shows the amount of data sent and received by the system.
- System Load: This column displays the load average of the CPU over the past 1, 5, and 15 minutes. 

Some additional options that can be used with the "dstat" command include:

- -c: This option displays only CPU usage statistics. 
- -d: This option displays only disk activity statistics. 
- -n: This option displays only network traffic statistics. 
- -f: This option displays the file system statistics. 

Overall, the dstat command is a powerful tool that is useful when monitoring system resources on a Linux machine. It is commonly used by system administrators to diagnose performance issues, troubleshoot bottlenecks, and monitor resource usage in real-time. 

## tldr 
 
> Versatile tool for generating system resource statistics.
> More information: <http://dag.wieers.com/home-made/dstat>.

- Display CPU, disk, net, paging and system statistics:

`dstat`

- Display statistics every 5 seconds and 4 updates only:

`dstat {{5}} {{4}}`

- Display CPU and memory statistics only:

`dstat --cpu --mem`

- List all available dstat plugins:

`dstat --list`

- Display the process using the most memory and most CPU:

`dstat --top-mem --top-cpu`

- Display battery percentage and remaining battery time:

`dstat --battery --battery-remain`
