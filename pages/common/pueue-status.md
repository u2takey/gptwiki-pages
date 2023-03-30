# pueue status 
## chatgpt 
The "pueue status" command is used to check the status of all the tasks that are added to a queue by the user. This command provides a summary of the tasks that are running, waiting or failed.

When the "pueue status" command is executed, it will display the following information for each task:

- Task ID: The unique ID of the task in the queue.
- Task Name: The name of the task.
- Status: The current status of the task which can be "queued", "running", "done" or "failed".
- Command: The command that needs to be executed.
- Log: A link to the log file of the task.

In addition to displaying the status of each task, the "pueue status" command also shows:

- The total number of tasks in the queue.
- The number of running tasks.
- The number of failed tasks.
- The number of completed tasks.

The "pueue status" command is useful for checking the progress of multiple tasks in the queue at once, and identifying any tasks that have failed or are currently running. 

## tldr 
 
> Display the current status of all tasks.
> More information: <https://github.com/Nukesor/pueue>.

- Show the status of all tasks:

`pueue status`

- Show the status of a specific group:

`pueue status --group {{group_name}}`
