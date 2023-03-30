# pueue restart 
## chatgpt 
The "pueue restart" command initiates a restart of all currently running tasks within the Pueue task manager. 

Pueue is a command-line task manager for managing long-running shell commands or scripts, allowing multiple tasks to run simultaneously and efficiently. This command is used to restart any interrupted or paused tasks. It essentially kills all currently running tasks and starts them again, which can help resolve errors or problems that have occurred during processing.

When you issue the "pueue restart" command, the Pueue task manager will send a signal to all currently running tasks, asking them to stop. After all the tasks have stopped, the manager will issue a start command to each one individually, which will start them up again from the beginning. 

Overall, running "pueue restart" ensures that any errors or problems with processes are resolved, and helps to ensure that all tasks are running efficiently and accurately to completion. 

## tldr 
 
> Restart tasks.
> More information: <https://github.com/Nukesor/pueue>.

- Restart a specific task:

`pueue restart {{task_id}}`

- Restart multiple tasks at once, and start them immediately (do not enqueue):

`pueue restart --start-immediately {{task_id}} {{task_id}}`

- Restart a specific task from a different path:

`pueue restart --edit-path {{task_id}}`

- Edit a command before restarting:

`pueue restart --edit {{task_id}}`

- Restart a task in-place (without enqueuing as a separate task):

`pueue restart --in-place {{task_id}}`

- Restart all failed tasks and stash them:

`pueue restart --all-failed --stashed`
