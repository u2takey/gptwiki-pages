# pueue switch 
## chatgpt 
The "pueue switch" command is a command used in the Pueue task manager in Linux. It is used to switch the currently running task with another task that has been paused in the Pueue queue.

When you have multiple tasks queued in Pueue and one is already running, you might want to switch the currently running task with another task in the queue. To do this, you would use the "pueue switch" command.

The basic syntax of the "pueue switch" command is as follows:

```
pueue switch
```

This command will immediately switch the currently running task to the next paused task in the queue. The previously running task will be paused and the next task in the queue will start running.

The "pueue switch" command also has several options that can be used to customize its behavior. For example, you can specify which specific task in the queue should be switched with the currently running task, by specifying the task ID:

```
pueue switch <task_id>
```

You can also use the "--all" option to switch all paused tasks in the queue with the currently running task:

```
pueue switch --all
```

Overall, the "pueue switch" command is a useful tool for managing multiple tasks in the Pueue queue and quickly switching between them as needed. 

## tldr 
 
> Switches the queue position of two enqueued or stashed commands.
> More information: <https://github.com/Nukesor/pueue>.

- Switch the priority of two tasks:

`pueue switch {{task_id1}} {{task_id2}}`
