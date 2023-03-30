# pueue stash 
## chatgpt 
The "pueue stash" command is used to temporarily save the current task queue of the Pueue task manager in a stash. This is useful when you want to pause a running task queue temporarily and resume it later.

When you run the "pueue stash" command, Pueue will save the current state of the task queue to a stash file, remove all tasks from the current queue, and leave them in the stash. You can later recall the tasks and continue execution from where it was paused.

Here are the steps to use the "pueue stash" command:

1. Open a terminal window and ensure that the Pueue task manager is running.

2. Run the command "pueue stash".

3. All the tasks currently in the queue will be removed and saved in the stash file.

4. The next time you want to resume the queue, use the "pueue restore" command to restore the queue from the stash file.

Note that stashing the queue does not kill or stop any running tasks. If you want to pause a running task, you will need to use the "pueue stop" command to stop it first, and then use "pueue stash" to save the current queue.

To summarize, "pueue stash" is a command that allows you to save the current state of the Pueue task queue to a stash file, and remove all tasks from the current queue. You can later restore the queue from the stash file and continue execution from where it was paused. 

## tldr 
 
> Stash tasks to prevent them starting automatically.
> See also `pueue start` and `pueue enqueue`.
> More information: <https://github.com/Nukesor/pueue>.

- Stash an enqueued task:

`pueue stash {{task_id}}`

- Stash multiple tasks at once:

`pueue stash {{task_id}} {{task_id}}`

- Start a stashed task immediately:

`pueue start {{task_id}}`

- Enqueue a task to be executed when preceding tasks finish:

`pueue enqueue {{task_id}}`
