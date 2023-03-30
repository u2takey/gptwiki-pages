# renice 
## chatgpt 
The command "renice" is used to change the priority of a running process. In Unix-based systems, processes are assigned a priority value by the scheduler, which determines the amount of CPU time they are allotted. The renice command allows a user to adjust the priority of a process so that it receives either more or less CPU time, depending on the user's needs.

The syntax for the renice command is:

renice priority [pid1] [pid2] [...]

The "priority" parameter specifies the new priority value, which is a numerical value ranging from -20 (highest priority) to 19 (lowest priority). The process ID (pid) of the process(es) whose priority is to be changed is also specified in the command, either by specifying a single PID or a list of PIDs separated by spaces.

For example, to increase the priority of process ID 123 to -10, the command would be:

renice -10 123

This would cause the process to receive more CPU time, potentially making it run faster. Conversely, to decrease the priority of process ID 456 to 10, the command would be:

renice 10 456

This would cause the process to receive less CPU time, potentially making it run slower.

In summary, the renice command allows a user to adjust the priority of a running process to optimize system performance and meet their specific needs. 

## tldr 
 
> Alters the scheduling priority/niceness of one or more running processes.
> Niceness values range from -20 (most favorable to the process) to 19 (least favorable to the process).
> More information: <https://manned.org/renice>.

- Change priority of a running process:

`renice -n {{niceness_value}} -p {{pid}}`

- Change priority of all processes owned by a user:

`renice -n {{niceness_value}} -u {{user}}`

- Change priority of all processes that belong to a process group:

`renice -n {{niceness_value}} --pgrp {{process_group}}`
