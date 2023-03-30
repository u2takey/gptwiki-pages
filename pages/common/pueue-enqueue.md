# pueue enqueue 
## chatgpt 
The `pueue enqueue` command is used in the Pueue task manager to add a new command or script to the task queue. When the command is added, it will be executed in the order it was added, after all previously added tasks have completed.

Here's how to use `pueue enqueue`:

1. Open the terminal on your computer and type `pueue enqueue` followed by the task you want to add to the queue.

2. You can add a single command or a complex script. You can also add multiple tasks at once, separated by spaces.

3. Once you've added all the tasks to the queue, you can check the status of the queue by using the `pueue status` command.

4. The tasks will be executed in the order they were added, one at a time. If a task fails, it will be stopped and the next task will start.

The `pueue enqueue` command is useful for managing workflows or running long tasks that require minimal interaction from the user. By adding tasks to the queue, you can be sure that they will be executed in the order you want and without interruption. 

## tldr 
 
> Enqueue stashed tasks.
> See also: `pueue stash`.
> More information: <https://github.com/Nukesor/pueue>.

- Enqueue multiple stashed tasks at once:

`pueue enqueue {{task_id}} {{task_id}}`

- Enqueue a stashed task after 60 seconds:

`pueue enqueue --delay {{60}} {{task_id}}`

- Enqueue a stashed task next Wednesday:

`pueue enqueue --delay {{wednesday}} {{task_id}}`

- Enqueue a stashed task after four months:

`pueue enqueue --delay "4 months" {{task_id}}`

- Enqueue a stashed task on 2021-02-19:

`pueue enqueue --delay {{2021-02-19}} {{task_id}}`

- List all available date/time formats:

`pueue enqueue --help`
