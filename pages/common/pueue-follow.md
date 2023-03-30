# pueue follow 
## chatgpt 
The "pueue follow" command is used to follow the output of a running task in Pueue.

Pueue is a process manager that allows users to manage and execute their command-line tasks efficiently. It allows users to queue their tasks and run them in the order they were added. The "pueue follow" command allows users to follow the output of a running task. When a task is running, it may produce output to the console. With the "pueue follow" command, users can see this output in real-time.

To use the "pueue follow" command, the user must have a task that is already running. The user can select the task by its index or by its name. Once a task is selected, the user can use the "pueue follow" command to follow the output of the task.

When the "pueue follow" command is executed, the output of the selected task will be displayed in real-time on the console. If the task produces additional output, it will be added to the console output in real-time. The user can stop following the task's output by pressing "Ctrl + C" on their keyboard.

In summary, the "pueue follow" command is used to follow the output of a running task in Pueue. It allows users to see the console output of a running task in real-time. 

## tldr 
 
> Follow the output of a currently running task.
> See also: `pueue log`.
> More information: <https://github.com/Nukesor/pueue>.

- Follow the output of a task (`stdout` + `stderr`):

`pueue follow {{task_id}}`

- Follow the `stderr` of a task:

`pueue follow --err {{task_id}}`
