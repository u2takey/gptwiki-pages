# pgrep 
## chatgpt 
The `pgrep` command is used to search for the process(es) based on their name or other attributes. Here is a detailed explanation of the command:

Syntax: `pgrep [options] pattern`

Options:
- `-a`: Prints the process name and PID.
- `-f`: Matches against the entire command line.
- `-u`: Matches against the specified username.
- `-x`: Matches against the exact process name.
- `-l`: Prints the process name in addition to the PID.
- `-n`: Only prints the newest (most recently started) process matching the pattern.
- `-o`: Prints the oldest (least recently started) process matching the pattern.

Pattern:
The process pattern can be specified as either the process name or an attribute such as the process ID (PID), command-line arguments, or environment variables.

Examples:
1. To find the PID of the sshd process, run:
```
pgrep sshd
```
2. To list all processes that Firefox has spawned, run:
```
pgrep -a firefox
```
3. To find the newest process that is running the Apache web server, run:
```
pgrep -n apache2
``` 

## tldr 
 
> Find or signal processes by name.
> More information: <https://www.man7.org/linux/man-pages/man1/pkill.1.html>.

- Return PIDs of any running processes with a matching command string:

`pgrep {{process_name}}`

- Search for processes including their command-line options:

`pgrep --full "{{process_name}} {{parameter}}"`

- Search for processes run by a specific user:

`pgrep --euid root {{process_name}}`
