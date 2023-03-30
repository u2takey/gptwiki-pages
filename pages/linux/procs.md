# procs 
## chatgpt 
As an AI language model, I must clarify that the answer largely depends on the context of where the command "procs" is being utilized. However, I can try to give an explanation of the command "procs" in general:

The command "procs" is short for "processes" in Unix/Linux systems. It is used to display information about the running processes on the system. When executed, the "procs" command will list information about each process being executed, such as the process ID (PID), the user who initiated the process, the amount of CPU and memory resources being used by the process, and the current status of the process.

This command is used by system administrators or users to monitor and manage the system's performance and resources. It can help in identifying any process that is consuming excessive resources and slowing down the system. The output can also be used to analyze the different components of a process to better understand how an application works, such as its dependencies and usage patterns.

Overall, the "procs" command can be used to obtain essential details about the currently running processes in the Unix/Linux system and present them in a concise format, aiding in system administration and troubleshooting. 

## tldr 
 
> Display information about the active processes.
> More information: <https://github.com/dalance/procs>.

- List all processes showing the PID, user, CPU usage, memory usage, and the command which started them:

`procs`

- List information about processes, if the commands which started them contain `zsh`:

`procs {{zsh}}`

- List information about all processes sorted by CPU time in [a]scending or [d]escending order:

`procs {{--sorta|--sortd}} cpu`

- List information about processes with either a PID, command, or user containing `41` or `firefox`:

`procs --or {{PID|command|user}} {{41}} {{firefox}}`

- List information about processes with both PID `41` and a command or user containing `zsh`:

`procs --and {{41}} {{zsh}}`
