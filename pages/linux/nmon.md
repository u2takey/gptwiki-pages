# nmon 
## chatgpt 
The command "nmon" is a performance monitoring tool that collects various system statistics including CPU, memory, disk, network activity, and many more. It stands for "Nigel's Monitor" and was originally developed for AIX (IBM's Unix operating system) systems, but can now be used on various Linux distributions as well.

To use the nmon command, you can simply type "nmon" in the terminal and it will launch an interactive dashboard displaying various system statistics in real-time. The dashboard is divided into multiple sections, with each section representing a different system component. By default, nmon displays CPU utilization, memory usage, top processes, and disks I/O activity.

In addition to displaying real-time system stats, nmon also provides an option to save data to a file for later analysis using the -f flag. By specifying a filename, nmon will generate a CSV file containing all the data collected during a certain period, which can be useful for identifying system bottlenecks, analyzing performance trends, and troubleshooting issues.

Overall, nmon is a powerful and user-friendly performance monitoring tool that can help system administrators and developers effectively manage and optimize their systems. 

## tldr 
 
> A system administrator, tuner, and benchmark tool.
> More information: <https://manned.org/nmon>.

- Start nmon:

`nmon`

- Save records to file ("-s 300 -c 288" by default):

`nmon -f`

- Save records to file with a total of 240 measurements, by taking 30 seconds between each measurement:

`nmon -f -s {{30}} -c {{240}}`
