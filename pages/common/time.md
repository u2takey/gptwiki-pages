# time 
## chatgpt 
The `time` command is a Linux utility that measures the amount of time it takes for a command to execute. When you run a command with the `time` command, it shows a summary of the resources used by the command, such as CPU time, system time, and wall-clock time.

Here's the syntax and usage of the `time` command:

```
time [option] command [arguments]
```

- `option`: It is an optional argument that can be used to modify the behavior of the `time` command. Some of the commonly used options are `-p` (provides POSIX format output), `-f` (provides user-defined format output), and `-v` (provides verbose output)
- `command`: It is the command that you want to run.
- `arguments`: These are the optional arguments that can be passed to the command.

When you run the `time` command, it outputs the following information:

- `real`: It shows the actual amount of time taken by the command to execute from start to finish.
- `user`: It shows the amount of time that the CPU spends running the command in user mode.
- `sys`: It shows the amount of time that the CPU spends running the command in kernel mode.
- `%CPU`: It shows the percentage of CPU time used by the command.

In summary, the `time` command is used to measure the execution time of a command and provides useful information on the resources used by the command. It's a simple and useful tool for measuring the performance of different commands and scripts. 

## tldr 
 
> See how long a command takes.
> More information: <https://manned.org/time>.

- Time "ls":

`time ls`
