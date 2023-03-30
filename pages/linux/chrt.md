# chrt 
## chatgpt 
The "chrt" command is a Linux/Unix command used to set the scheduling priority of a process. It stands for "change real-time scheduling priority". It is commonly used by system administrators to improve the performance of critical processes by changing their priority level.

The basic syntax of the chrt command is:

chrt [options] priority command [args]

The "options" field allows you to specify additional options, such as the scheduling policy to use. The "priority" field specifies the priority level, with lower values indicating higher priority. The "command" field specifies the name of the command to run, and the "args" field specifies any arguments to the command.

The "priority" field can be specified using one of several values, such as:

- -r: Set real-time priority (1-99)
- -f: Set FIFO scheduling priority (1-99)
- -b: Set batch scheduling priority (0-14)
- -i: Set idle scheduling priority (0)
- -o: Set other scheduling policy (default)

For example, the following command sets the priority of the "myscript.sh" script to 50 using the FIFO scheduling policy:

chrt -f 50 ./myscript.sh

This will ensure that the "myscript.sh" process is given the highest priority by the Linux scheduler, and any other processes will be pre-empted in favor of it.

Overall, the "chrt" command is a powerful tool for optimizing the performance of critical processes in Linux/Unix systems, but it should be used with caution and only by experienced system administrators. 

## tldr 
 
> Manipulate the real-time attributes of a process.
> More information: <https://man7.org/linux/man-pages/man1/chrt.1.html>.

- Display attributes of a process:

`chrt --pid {{PID}}`

- Display attributes of all threads of a process:

`chrt --all-tasks --pid {{PID}}`

- Display the min/max priority values that can be used with `chrt`:

`chrt --max`

- Set the scheduling policy for a process:

`chrt --pid {{PID}} --{{deadline|idle|batch|rr|fifo|other}}`
