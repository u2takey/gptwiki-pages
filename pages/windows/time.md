# time 
## chatgpt 
The "time" command is a system command used to measure the execution time of a command or a shell script in Linux. 

When the "time" command is used without any arguments, it simply runs a command or program and provides information about the time taken to run the command. 

For example, if you run the command "time ls -l" in the terminal, it will output something like:

```
real    0m0.005s
user    0m0.002s
sys     0m0.002s
```

Here, "real" represents the actual time taken for the command to run, "user" is the amount of CPU time spent running the command in user mode, and "sys" is the amount of CPU time spent running the command in kernel mode.

Apart from this, the "time" command also has a few options that can be used to customize the output, such as "-f" to specify a custom format string, "-p" to output in a format that can be parsed by other programs, and "-o" to redirect output to a file. 

Overall, the "time" command is a useful tool for measuring the performance of a command or script, and can help identify any bottlenecks or areas for optimization. 

## tldr 
 
> Display or set the system time.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/time>.

- Display the current system time and prompt to enter a new time (leave empty to keep unchanged):

`time`

- Display the current system time without prompting for a new time:

`time /t`
