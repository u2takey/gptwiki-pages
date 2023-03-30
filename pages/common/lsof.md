# lsof 
## chatgpt 
The "lsof" command stands for "list open files" and is used to gather information about currently opened files and processes in a system. When executed without any arguments, the "lsof" command displays a list of all open files and sockets on the system. This information includes process IDs, usernames, file descriptors, file types, file modes, and file paths.

The output of the "lsof" command can be customized using various command-line options. Some common options and their uses include:

- -p: limits the display to a specific process ID
- -u: limits the display to a specific user
- -i: limits the display to a specific network port or address
- -c: limits the display to a specific command name
- -n: disables the conversion of network addresses to hostnames

The "lsof" command can be useful for troubleshooting issues related to file or network access, identifying which processes are using specific files or ports, and monitoring system activity. However, as it gathers sensitive information about running processes, it is important to use the "lsof" command with caution and only as needed. 

## tldr 
 
> Lists open files and the corresponding processes.
> Note: Root privileges (or sudo) is required to list files opened by others.
> More information: <https://manned.org/lsof>.

- Find the processes that have a given file open:

`lsof {{path/to/file}}`

- Find the process that opened a local internet port:

`lsof -i :{{port}}`

- Only output the process ID (PID):

`lsof -t {{path/to/file}}`

- List files opened by the given user:

`lsof -u {{username}}`

- List files opened by the given command or process:

`lsof -c {{process_or_command_name}}`

- List files opened by a specific process, given its PID:

`lsof -p {{PID}}`

- List open files in a directory:

`lsof +D {{path/to/directory}}`

- Find the process that is listening on a local IPv6 TCP port and don't convert network or port numbers:

`lsof -i6TCP:{{port}} -sTCP:LISTEN -n -P`
