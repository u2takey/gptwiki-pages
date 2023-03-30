# pueue log 
## chatgpt 
The `pueue log` command is used in the Pueue task manager to display the logs of all tasks that have been executed or are currently running.

When run, it displays a table of all tasks along with their log status, exit status, start and end time, and the command that was run. The log status column shows the number of lines of log output that have been written so far, and the exit status column shows the status code returned by the task when it completed.

If you want to see the log output of a particular task, you can use the command `pueue log <task_id>` where `<task_id>` is the ID of the task you want to view the log of. This will display the detailed log output for that task.

You can also use various flags with the `pueue log` command to filter the output by status, limit the number of lines displayed, or show only the most recent logs. For example, `pueue log -s success` will show only the log output for tasks that completed successfully, while `pueue log --tail 10` will show only the last 10 lines of the log output for each task. 

In summary, the `pueue log` command is a useful tool for monitoring the status and output of tasks managed by Pueue. 

## tldr 
 
> Display the log output of 1 or more tasks.
> See also: `pueue status`.
> More information: <https://github.com/Nukesor/pueue>.

- Show the last few lines of output from all tasks:

`pueue log`

- Show the full output of a task:

`pueue log {{task_id}}`

- Show the last few lines of output from several tasks:

`pueue log {{task_id}} {{task_id}}`

- Print a specific number of lines from the tail of output:

`pueue log --lines {{number_of_lines}} {{task_id}}`
