# pueue remove 
## chatgpt 
The "pueue remove" command is used in the Pueue task manager to remove a specific task from the task queue. 

When executed, the command will prompt the user to enter the ID of the task they want to remove. Once the ID is entered, the task will be removed from the queue and any associated resources (such as files or processes) will also be terminated.

It's important to note that the "pueue remove" command will only remove a single task from the queue. If you want to remove multiple tasks, you'll need to execute the command multiple times. 

Additionally, if a task is already running, you may need to use the "pueue kill" command to terminate it before you can remove it from the queue using the "pueue remove" command. 

Overall, the "pueue remove" command is a useful tool for managing your task queue and ensuring that your system resources are being used efficiently. 

## tldr 
 
> Remove tasks from the list. Running or paused tasks need to be killed first.
> More information: <https://github.com/Nukesor/pueue>.

- Remove a killed or finished task:

`pueue remove {{task_id}}`

- Remove multiple tasks at once:

`pueue remove {{task_id}} {{task_id}}`
