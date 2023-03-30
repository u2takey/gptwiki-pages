# bpytop 
## chatgpt 
bpytop is a command-line utility for monitoring system resources in real-time. It provides an interactive and customizable interface that displays the system's CPU usage, memory usage, disk I/O operations, and network activity. By default, it shows the most active processes and their resource consumption.

When executed, bpytop opens a terminal window with a dashboard-style view of the system resources. The dashboard can be configured to show or hide various information, such as system load, CPU temperature, and disk space usage. It also allows you to sort and filter the displayed data based on various metrics such as high CPU usage or high memory usage.

Additionally, bpytop provides several keyboard shortcuts that enable you to interact with the displayed data, such as selecting and killing processes, adjusting display settings, and filtering data. These shortcuts make navigating the dashboard and managing system resources much easier and faster.

Overall, bpytop is an excellent utility for monitoring system resources and diagnosing performance problems. It is suitable for both experienced users and beginners who want a quick and easy way to visualize their system's processes and resource consumption. 

## tldr 
 
> Display dynamic real-time information about running processes with graphs. Similar to `gtop` and `htop`.
> More information: <https://github.com/aristocratos/bpytop>.

- Start bpytop:

`bpytop`

- Start in minimal mode without memory and networking boxes:

`bpytop -m`

- Show version:

`bpytop -v`

- Toggle minimal mode:

`m`

- Search for running programs or processes:

`f`

- Change settings:

`M`
