# watch 
## chatgpt 
watch is a command that continuously runs a specified command or shell script and displays its output in real time. It is mainly used to monitor changes in system processes, files, or directories.

The syntax of the watch command is:

watch [options] command

Options:
- -n or --interval: specifies the time interval (in seconds) between each update of the output. The default interval is 2 seconds.
- -d or --differences: highlights the differences between each update of the output.

Command: specifies the command or shell script to be monitored.

Example:

watch -n 5 ps -ef

This command will monitor the system processes every 5 seconds and display the output of the ps -ef command in real time.

Note: The watch command is not available on all operating systems. It is mainly used on Linux or Unix-based systems. 

## tldr 
 
> Execute a command repeatedly, and monitor the output in full-screen mode.
> More information: <https://manned.org/watch>.

- Monitor files in the current directory:

`watch {{ls}}`

- Monitor disk space and highlight the changes:

`watch -d {{df}}`

- Monitor "node" processes, refreshing every 3 seconds:

`watch -n {{3}} "{{ps aux | grep node}}"`
