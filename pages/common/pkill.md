# pkill 
## chatgpt 
pkill is a command used in Unix-based operating systems to kill one or more processes based on their name or other attributes. The word "pkill" is derived from the "kill process" command. 

The syntax for the pkill command is as follows:

pkill [OPTIONS] PATTERN

- OPTIONS: Specify optional parameters for the command.
- PATTERN: Specify the name or other attribute of the process(es) to be killed.

Examples of the pkill command:

1. To kill a process with a specific name, use the following command:
   pkill firefox
   This command would kill all running Firefox processes.

2. To kill all processes owned by a specific user, use the following command:
   pkill -u username
   This command would kill all processes owned by the specified user.

3. To send a specific signal to a process, use the following command:
   pkill -SIGTERM firefox
   This command would send the SIGTERM signal to all running Firefox processes.

In summary, pkill is a useful command for killing one or more processes based on their name, ownership, or other attributes. It offers several options and allows for precise control over the processes to be killed. 

## tldr 
 
> Signal process by name.
> Mostly used for stopping processes.
> More information: <https://www.man7.org/linux/man-pages/man1/pkill.1.html>.

- Kill all processes which match:

`pkill "{{process_name}}"`

- Kill all processes which match their full command instead of just the process name:

`pkill -f "{{command_name}}"`

- Force kill matching processes (can't be blocked):

`pkill -9 "{{process_name}}"`

- Send SIGUSR1 signal to processes which match:

`pkill -USR1 "{{process_name}}"`

- Kill the main `firefox` process to close the browser:

`pkill --oldest "{{firefox}}"`
