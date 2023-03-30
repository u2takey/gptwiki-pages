# pueue pause 
## chatgpt 
The `pueue pause` command is used to pause a running task or multiple tasks in Pueue, which is a command-line task manager for sequential and parallel task execution. 

When this command is executed, it sends the pause signal to a specified task or group of tasks, which causes them to suspend their execution at the current point, and they will not continue until the corresponding `pueue resume` command is given. 

The syntax for the `pueue pause` command is:

```
pueue pause [TASK_ID] [...]
```

If no argument is provided, it pauses all running tasks. Otherwise, you need to specify the task IDs for the tasks that you want to pause.

For example, to pause a task with ID 3, run:

```
pueue pause 3
```

If there are multiple tasks you want to pause, you can specify all their IDs, separated by spaces:

```
pueue pause 3 5 7
```

Once the specified tasks are paused, you can use the `pueue status` command to check their current status. The paused tasks will be listed under the "paused" section. 

Note that if a task is already in a failed or finished state, it cannot be paused. 

In summary, this command is useful for temporarily interrupting the execution of a task or group of tasks in Pueue, which allows you to manage them more effectively if you need to prioritize other tasks or resolve potential issues. 

## tldr 
 
> Pause running tasks or groups.
> See also: `pueue start`.
> More information: <https://github.com/Nukesor/pueue>.

- Pause all tasks in the default group:

`pueue pause`

- Pause a running task:

`pueue pause {{task_id}}`

- Pause a running task and stop all its direct children:

`pueue pause --children {{task_id}}`

- Pause all tasks in a group and prevent it from starting new tasks:

`pueue pause --group {{group_name}}`

- Pause all tasks and prevent all groups from starting new tasks:

`pueue pause --all`
