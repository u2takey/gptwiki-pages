# pueue reset 
## chatgpt 
The `pueue reset` command is used to reset all tasks in the Pueue task manager to the "queued" state, regardless of their current status. This means that any running or paused tasks will be stopped, and all tasks will be retried from the beginning when they are scheduled to run again.

This command is useful when you want to start fresh and ensure that all tasks are in a consistent and predictable state. It can also be used to address issues with tasks that are stuck or not completing properly.

Some additional options that can be used with the `pueue reset` command include:

- `--clean`: This option will also delete all task output files, logs, and queues.
- `--hard`: This option will stop all running tasks and delete all tasks from the queue. It effectively resets the Pueue task manager to an empty state.
- `--yes`: This option will skip the confirmation prompt and automatically reset all tasks.

Overall, the `pueue reset` command is a powerful tool for managing tasks in Pueue and ensuring that everything is running smoothly. 

## tldr 
 
> Kill everything and reset.
> More information: <https://github.com/Nukesor/pueue>.

- Kill all tasks and remove everything (logs, status, groups, task IDs):

`pueue reset`

- Kill all tasks, terminate their children, and reset everything:

`pueue reset --children`

- Reset without asking for confirmation:

`pueue reset --force`
