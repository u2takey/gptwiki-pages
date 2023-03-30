# top 
## chatgpt 
The "top" command is a tool used in UNIX/Linux systems that provides real-time process monitoring. When executed, it displays a continuously updating list of processes in order of their usage of system resources such as CPU usage, memory usage, and other related details.

Some of the basic options that can be used with the top command include:

- '-d': It specifies the amount of time (in seconds) the screen should refresh
- '-u': This option displays processes that belong to a specific user
- '-p': It displays information about a specific process ID (PID)
- '-H': This option shows the list of processes along with their child processes in a hierarchal structure
- '-o': This option sorts the list based on a chosen field, such as PID, CPU usage, or memory usage.

Overall, the "top" command is a helpful tool for system administrators and users to monitor system resource usage, identify resource-hogging programs, and troubleshoot performance issues. 

## tldr 
 
> Display dynamic real-time information about running processes.
> More information: <https://manned.org/top>.

- Start top:

`top`

- Do not show any idle or zombie processes:

`top -i`

- Show only processes owned by given user:

`top -u {{username}}`

- Sort processes by a field:

`top -o {{field_name}}`

- Show the individual threads of a given process:

`top -Hp {{process_id}}`

- Show only the processes with the given PID(s), passed as a comma-separated list. (Normally you wouldn't know PIDs off hand. This example picks the PIDs from the process name):

`top -p $(pgrep -d ',' {{process_name}})`

- Get help about interactive commands:

`?`
