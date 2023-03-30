# nohup 
## chatgpt 
The `nohup` command is used to execute a command or a shell script in a way that it continues running even after the user exits the terminal session. It stands for "no hang up" and is particularly useful when a long-running process needs to be executed on a remote server, and shutting down the client computer or closing the terminal window would normally terminate the process.

The command syntax for `nohup` is as follows:
```
nohup command [arg...]
```
Where `command` is the command or script to be executed and `arg` refers to any command-line arguments to be passed to the command.

When a command or script is executed with `nohup`, it redirects its standard input, output, and error streams so that they are attached to a file named `nohup.out`. This file is created in the same directory as the shell script, except for situations where the user does not have write access to the current directory, in which case the file is created in the user's home directory.

Once a command or script is running with `nohup`, the user can safely exit the terminal session without worrying about accidentally terminating the process. The process will continue to run in the background until it completes or is forcefully terminated.

It is worth noting that while `nohup` can be used to keep a process running even when the user logs out or the terminal is closed, it does not prevent the process from being terminated by other means, such as a forced stop or shutdown of the server. 

## tldr 
 
> Allows for a process to live when the terminal gets killed.
> More information: <https://www.gnu.org/software/coreutils/nohup>.

- Run a process that can live beyond the terminal:

`nohup {{command}} {{argument1 argument2 ...}}`

- Launch `nohup` in background mode:

`nohup {{command}} {{argument1 argument2 ...}} &`

- Run a shell script that can live beyond the terminal:

`nohup {{path/to/script.sh}} &`

- Run a process and write the output to a specific file:

`nohup {{command}} {{argument1 argument2 ...}} > {{path/to/output_file}} &`
