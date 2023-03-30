# pueue edit 
## chatgpt 
The `pueue edit` command is used to edit a specific task that has been added to the pueue queue. 

Here is a breakdown of the command's syntax:

- `pueue`: This is the command used to interact with the pueue queue manager.
- `edit`: This is the subcommand that tells pueue to make modifications to an existing task.

When running the `pueue edit` command, you will need to specify which task you are editing by providing either the task's ID or its position in the queue. Once you have specified which task you want to edit, you will be prompted to make changes to the task's configuration, such as changing its command, adjusting its priority or setting its environment variables, before saving and exiting the editor.

The `pueue edit` command is helpful when you need to make changes to a task that has already been added to the queue but needs to be modified before running. This can save time and effort in having to delete and re-add tasks to the pueue queue. 

## tldr 
 
> Edit the command or path of a stashed or queued task.
> More information: <https://github.com/Nukesor/pueue>.

- Edit a task, see `pueue status` to get the task ID:

`pueue edit {{task_id}}`

- Edit the path from which a task is executed:

`pueue edit {{task_id}} --path`

- Edit a command with the specified editor:

`EDITOR={{nano}} pueue edit {{task_id}}`
