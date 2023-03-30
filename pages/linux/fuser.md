# fuser 
## chatgpt 
The `fuser` command is a command-line utility used in Unix-based systems to identify processes that are currently using a particular file or directory. 

The command takes one or more filenames or directory names as arguments, and displays the PIDs (Process IDs) of the processes that have opened these files or directories. 

The syntax of the command is as follows:

```
fuser [options] [file(s)/directory(s)]
```

Here are some of the most commonly used options with the `fuser` command:

- `-k`: This option is used to send a signal to the processes using the file(s)/directory(s), which will terminate them. For example, `fuser -k /var/log/messages` will kill all the processes that are using the `/var/log/messages` file.

- `-u`: This option is used to display the usernames of the processes using the file(s)/directory(s). For example, `fuser -u /var/log/messages` will display the usernames of the processes using the `/var/log/messages` file.

- `-v`: This option is used to display verbose output, which includes the process IDs and the full command line of the processes using the file(s)/directory(s).

Here is an example of using the `fuser` command to display the PIDs of processes using the `/var/log/messages` file:

```
$ fuser /var/log/messages
/var/log/messages:   1262  2125  2126  3009  3010
```

In the above example, the output displays the PIDs of five processes currently using the `/var/log/messages` file. 

Overall, the `fuser` command can be a useful tool for troubleshooting issues that may arise when files or directories are locked, and to help identify processes that are causing the issue. 

## tldr 
 
> Display process IDs currently using files or sockets.
> More information: <https://manned.org/fuser>.

- Find which processes are accessing a file or directory:

`fuser {{path/to/file_or_directory}}`

- Show more fields (`USER`, `PID`, `ACCESS` and `COMMAND`):

`fuser --verbose {{path/to/file_or_directory}}`

- Identify processes using a TCP socket:

`fuser --namespace tcp {{port}}`

- Kill all processes accessing a file or directory (sends the `SIGKILL` signal):

`fuser --kill {{path/to/file_or_directory}}`

- Find which processes are accessing the filesystem containing a specific file or directory:

`fuser --mount {{path/to/file_or_directory}}`

- Kill all processes with a TCP connection on a specific port:

`fuser --kill {{port}}/tcp`
