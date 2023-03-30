# sleep 
## chatgpt 
The sleep command is a system command which is used to pause the execution of a script or batch file for a specified amount of time in seconds, minutes, hours, or days. It is used to create delays in the shell scripts and batch files.

The basic syntax of the sleep command in Linux is:

```sleep [time]```

Where [time] is the amount of time that the script must sleep.

For example, to pause the script execution for 5 seconds, you can use the following command:

```sleep 5```

The sleep command can also accept fractional time values. For instance:

```sleep 1.5```

This command will pause the script for 1.5 seconds before continuing the execution.

Depending on the operating system, the sleep command may have additional options. For instance, on some systems, the -m option can be used to specify time in milliseconds instead of seconds:

```sleep -m 500```

This command will pause the script for 500 milliseconds (0.5 seconds) before continuing the execution.

Overall, the sleep command is a simple yet effective way to control the time delay between commands in shell scripts and batch files. 

## tldr 
 
> Delay for a specified amount of time.
> More information: <https://www.gnu.org/software/coreutils/sleep>.

- Delay in seconds:

`sleep {{seconds}}`

- Delay in [m]inutes. (Other units [d]ay, [h]our, [s]econd, [inf]inity can also be used):

`sleep {{minutes}}m`

- Delay for 1 [d]ay 3 [h]ours:

`sleep 1d 3h`

- Execute a specific command after 20 [m]inutes delay:

`sleep 20m && {{command}}`
