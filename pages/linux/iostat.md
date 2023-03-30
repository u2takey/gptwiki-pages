# iostat 
## chatgpt 
The iostat command is a tool for monitoring system input/output (I/O) statistics for devices and partitions. When executed, it displays various information related to disk usage such as CPU utilization, I/O rates, and transfer time. The iostat command provides users with real-time information about the performance of storage devices and can help to identify bottlenecks in disk I/O.

The basic syntax of the iostat command is as follows:

iostat [options] [interval] [count]

Options:

- -c: Display only CPU statistics
- -d: Display only device statistics
- -k: Display results in kilobytes per second
- -m: Display results in megabytes per second
- -t: Display the time with each report
- -x: Display extended statistics

Interval: The interval specifies the amount of time in seconds between each report.

Count: The count specifies the number of reports to generate before exiting.

When running the iostat command, it displays the following columns of information:

- Device: The name of the device being monitored
- rrqm/s: The number of read requests merged per second
- wrqm/s: The number of write requests merged per second
- r/s: The number of read requests completed per second
- w/s: The number of write requests completed per second
- rkB/s: The number of kilobytes read per second
- wkB/s: The number of kilobytes written per second
- avgrq-sz: The average size of the requests
- avgqu-sz: The average queue length of the requests
- await: The average wait time for I/O requests
- svctm: The average service time for I/O requests
- %util: The percentage of time the device was busy completing requests.

By analyzing the data from the iostat command, system administrators can identify the disks that are experiencing the highest levels of usage and optimize the system to improve performance. 

## tldr 
 
> Report statistics for devices and partitions.
> More information: <https://manned.org/iostat>.

- Display a report of CPU and disk statistics since system startup:

`iostat`

- Display a report of CPU and disk statistics with units converted to megabytes:

`iostat -m`

- Display CPU statistics:

`iostat -c`

- Display disk statistics with disk names (including LVM):

`iostat -N`

- Display extended disk statistics with disk names for device "sda":

`iostat -xN {{sda}}`

- Display incremental reports of CPU and disk statistics every 2 seconds:

`iostat {{2}}`
