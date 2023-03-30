# systemd-analyze 
## chatgpt 
The `systemd-analyze` command is a system utility tool that is used to analyze the boot-up performance of Linux systems. It provides extensive information on the time taken by each service or application to start during the system boot process and helps users to identify any bottlenecks that might be causing delays in the boot-up process.

When the `systemd-analyze` command is run with no arguments, it provides a summary of the boot-up time, including the time taken to reach the graphical user interface (GUI). Additionally, it provides information on the time taken to start each service, including details such as the service name, time taken, and whether it is started in parallel with other services.

Here are the most commonly used options for the `systemd-analyze` command:

- `blame`: This option displays a list of all services and the time taken to start them. The list is sorted from the longest to the shortest start time.
- `critical-chain`: This option displays a list of services that are critical to the boot process and their dependencies. The list is sorted based on the time taken to start each service, starting from the longest. This helps users to identify which services are slowing down the boot process and may need to be optimized or disabled.
- `time`: This option displays a detailed breakdown of the system boot-up time, including the firmware initialization, kernel initialization, and user space initialization. This option is useful in identifying which part of the boot process is causing a delay.

In summary, the `systemd-analyze` command is an essential tool for diagnosing boot-up performance issues in Linux systems. It provides valuable insight into the boot process and helps users to optimize and improve system performance. 

## tldr 
 
> Analyze and debug system manager.
> Show timing details about the boot process of units (services, mount points, devices, sockets).
> More information: <https://manned.org/systemd-analyze>.

- List time of each unit to start up:

`systemd-analyze blame`

- Print a tree of the time-critical chain of units:

`systemd-analyze critical-chain`

- Create an SVG file showing when each system service started, highlighting the time that they spent on initialization:

`systemd-analyze plot > {{path/to/file.svg}}`

- Plot a dependency graph and convert it to an SVG file:

`systemd-analyze dot | dot -T{{svg}} > {{path/to/file.svg}}`

- Show security scores of running units:

`systemd-analyze security`
