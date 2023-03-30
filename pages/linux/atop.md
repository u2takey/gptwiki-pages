# atop 
## chatgpt 
The `atop` command is a Linux program that provides system-level monitoring of various resources like CPU usage, memory consumption, disk activity, and network utilization. Atop is similar to other monitoring tools such as top and htop, but it offers additional features such as the ability to log and playback system activity, as well as provide comprehensive resource usage reports.

When you run the `atop` command without any options, it will display a real-time view of the system's resource usage. The output displays a list of running processes, their CPUs usage percentage, memory usage, disk I/O, and network activity.

Some common options for the `atop` command include:

- `-r` : Enables playback mode, which allows you to see a log of system activities that were recorded by atop.
- `-b` : Generate system reports in batch mode.
- `-n` : Sets the update interval in seconds for the output.
- `-c` : Display the command line arguments of the processes being monitored.

Overall, the `atop` command is an excellent tool to help system administrators diagnose and troubleshoot system performance issues. It provides timely, detailed, and granular insights into the system's resource usage, and it also archives system activity logs that can be useful in tracking down and understanding system problems. 

## tldr 
 
> Linux system and process monitor.
> More information: <https://manned.org/atop>.

- Start:

`atop`

- Start and display memory consumption for each process:

`atop -m`

- Start and display disk information:

`atop -d`

- Start and display background process information:

`atop -c`

- Start and display thread-specific resource utilization information:

`atop -y`

- Start and display the number of processes for each user:

`atop -au`

- Display help about interactive commands:

`?`
