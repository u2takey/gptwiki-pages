# ps 
## chatgpt 
The "ps" command is a command-line utility on Unix-like operating systems used to display information about the processes currently running on a system. 

The default output of the "ps" command includes various details about the processes such as:

- PID: the process ID
- TTY: the Terminal associated with the process
- TIME: the amount of CPU time used by the process
- CMD: the command used to start the process

The "ps" command also has different options that can be used to customize the output. Some commonly used options are:

- -a: displays information about all processes
- -u: displays detailed information about the user who started the process
- -x: displays information about all processes, including those not associated with a Terminal

Overall, the "ps" command is a useful tool for understanding the state of a Unix-like operating system and the processes running on it. 

## tldr 
 
> Information about running processes.
> More information: <https://manned.org/ps>.

- List all running processes:

`ps aux`

- List all running processes including the full command string:

`ps auxww`

- Search for a process that matches a string:

`ps aux | grep {{string}}`

- List all processes of the current user in extra full format:

`ps --user $(id -u) -F`

- List all processes of the current user as a tree:

`ps --user $(id -u) f`

- Get the parent PID of a process:

`ps -o ppid= -p {{pid}}`

- Sort processes by memory consumption:

`ps --sort size`
