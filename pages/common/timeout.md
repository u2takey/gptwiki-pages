# timeout 
## chatgpt 
The `timeout` command is a built-in command in Linux and other Unix-like operating systems that is used to set a time limit for executing other commands. The `timeout` command allows users to limit the amount of time that a command is allowed to run, and if the command exceeds the specified time limit, it will be terminated automatically.

The syntax of the `timeout` command is as follows:

```
timeout [OPTION] DURATION COMMAND [ARG]...
```

Where `OPTION` specifies the options for the command, `DURATION` specifies the time limit in seconds or other time units, and `COMMAND` and `ARG` are the command and arguments to be executed.

For example, the following command sets a time limit of 5 seconds for executing the `sleep` command:

```
timeout 5s sleep 10
```

This command will terminate after 5 seconds, even though the `sleep` command would normally wait for 10 seconds before completing.

Some common options for the `timeout` command include:

- `-k` or `--kill-after` - specify a time limit after which the command should be forcibly terminated if it has not already exited
- `-s` or `--signal` - specify a signal to send to the command when it exceeds the time limit
- `-v` or `--verbose` - display more information about the execution of the command
- `-h` or `--help` - display help information about the `timeout` command

Overall, the `timeout` command is a useful tool for managing the execution of long-running or potentially problematic commands, and can help prevent system resources from being tied up indefinitely. 

## tldr 
 
> Run a command with a time limit.
> More information: <https://www.gnu.org/software/coreutils/timeout>.

- Run `sleep 10` and terminate it, if it runs for more than 3 seconds:

`timeout {{3s}} {{sleep 10}}`

- Specify the signal to be sent to the command after the time limit expires. (By default, TERM is sent):

`timeout --signal {{INT}} {{5s}} {{sleep 10}}`
