# pueue kill 
## chatgpt 
The `pueue kill` command is used to forcefully terminate a running process or a group of running processes that were previously added to the Pueue task manager queue. 

When you issue the `pueue kill` command, Pueue sends a signal to the specified process or group of processes that instructs them to stop execution immediately. This signal is similar to the Ctrl+C or SIGINT signal that you can send to a process using the keyboard.

If you run `pueue kill` with no arguments, it terminates all running tasks managed by Pueue.

The command requires you to specify the `task ID` or `group name` of the running process(es) you wish to terminate. You can use the `pueue status` command to see a list of all the running tasks and their corresponding task IDs and group names.

It's important to note that forcefully terminating a process may cause data loss or other issues, depending on the nature of the process being terminated. Therefore, it is advisable to use the `pueue kill` command only as a last resort and try to gracefully stop processes first with the `pueue stop` or `pueue pause` commands. 

## tldr 
 
> Kill running tasks or whole groups.
> More information: <https://github.com/Nukesor/pueue>.

- Kill all tasks in the default group:

`pueue kill`

- Kill a specific task:

`pueue kill {{task_id}}`

- Kill a task and terminate all its child processes:

`pueue kill --children {{task_id}}`

- Kill all tasks in a group and pause the group:

`pueue kill --group {{group_name}}`

- Kill all tasks across all groups and pause all groups:

`pueue kill --all`
