# nice 
## chatgpt 
The `nice` command is used in Unix/Linux operating systems to adjust the priority level of a process. It is used to launch a process with a specified priority, under the control of either the superuser or the owner of the process. The priority level is a value from -20 to 19, where -20 is the highest possible priority and 19 is the lowest possible priority. 

The syntax of the `nice` command is as follows:

```
nice [-n LEVEL] command [ARG]
```

The options available for the `nice` command are:

- `-n`: Specify the priority level in the range from -20 to 19. A higher value of the priority level denotes a lower priority. Default priority is 10 for non-root users and 0 for root user.

The `command` and `ARG` parameters are the name of the command to be executed and its arguments.

The `nice` command is useful when you want to run a process in the background without it eating up all the system resources. For example, if you run a CPU-intensive process, it will take up a lot of CPU cycles, which will slow down your system. By running the process with a lower priority using the `nice` command, you can reduce the impact that it has on your system's performance. 

For example, the following command runs the `ls` command with a lower priority level of 15:

```
nice -n 15 ls -l
```

This will cause the `ls` command to run with a lower priority, allowing other processes to use the CPU cycles that would have been used by the `ls` command. 

## tldr 
 
> Execute a program with a custom scheduling priority (niceness).
> Niceness values range from -20 (the highest priority) to 19 (the lowest).
> More information: <https://www.gnu.org/software/coreutils/nice>.

- Launch a program with altered priority:

`nice -n {{niceness_value}} {{command}}`
