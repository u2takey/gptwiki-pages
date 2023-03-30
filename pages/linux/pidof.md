# pidof 
## chatgpt 
The command "pidof" is a Linux command used to display the process ID (PID) of a running program. It is used to find the PID of a process by its name. 

Syntax: 

pidof [options] [name]

where,

- [name]: Name of the process you want to find the PID of.
- [options]: Flags that can be used to modify the behavior of the command.

Some commonly used options are:

- "-s": Only find the PID of the oldest (lowest PID) process with the given name.
- "-c": Display the number of PIDs found.
- "-x": Only find PIDs of processes with the exact same name as the one specified.

Example: 

To find the PID of the Apache web server process, the following command can be used:

pidof apache

This will display the PID of the Apache process. If there are multiple Apache processes running, it will display all their PIDs separated by spaces.

To display the number of Apache processes running, use the "-c" option:

pidof -c apache

If you only want to find the PID of the oldest Apache process, use the "-s" option:

pidof -s apache 

## tldr 
 
> Gets the ID of a process using its name.
> More information: <https://manned.org/pidof>.

- List all process IDs with given name:

`pidof {{bash}}`

- List a single process ID with given name:

`pidof -s {{bash}}`

- List process IDs including scripts with given name:

`pidof -x {{script.py}}`

- Kill all processes with given name:

`kill $(pidof {{name}})`
