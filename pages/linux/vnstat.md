# vnstat 
## chatgpt 
The "vnstat" command is used to monitor and view network traffic statistics in Linux systems. When executed, it displays traffic information about the network interfaces present on the system. 

The information it displays includes:

- Total amount of data (both upload and download) transferred through the interface
- Average and maximum data rates
- Data usage over time (daily, monthly, and yearly)

The "vnstat" command requires root privileges to access detailed network statistics.

Here are some examples of "vnstat" command usage:

1. To view the network statistics for all interfaces, use the command: 

```
vnstat
```

2. To view the network statistics for a specific interface, specify the interface name as an argument. For example: 

```
vnstat -i eth0
```

3. To display network statistics in real-time continuously, use the command:

```
vnstat -l
```

4. To view hourly statistics for today, use the command: 

```
vnstat -h
```

5. To view monthly statistics, use the command: 

```
vnstat -m
```

Overall, the "vnstat" command provides a useful tool for monitoring and analyzing network traffic history and usage. It can help you identify network usage trends, optimize bandwidth consumption, and troubleshoot network issues. 

## tldr 
 
> A console-based network traffic monitor.
> More information: <https://manned.org/vnstat>.

- Display traffic summary for all interfaces:

`vnstat`

- Display traffic summary for a specific network interface:

`vnstat -i {{eth0}}`

- Display live stats for a specific network interface:

`vnstat -l -i {{eth0}}`

- Show traffic statistics on an hourly basis for the last 24 hours using a bar graph:

`vnstat -hg`

- Measure and show average traffic for 30 seconds:

`vnstat -tr {{30}}`
