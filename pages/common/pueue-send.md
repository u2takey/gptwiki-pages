# pueue send 
## chatgpt 
The "pueue send" command is a command used in the Pueue task manager. It is used to send a command to a running task or set of tasks that have been added to the Pueue queue. When run with the appropriate arguments, "pueue send" sends a command to a specific task or group of tasks, telling them what to do next. 

For example, you might use "pueue send" to tell a running task to pause, stop, or resume executing. You might also use it to send a new set of command line arguments to a running task, which could change its behavior or output.

In general, the "pueue send" command allows you to interact with running tasks in a more sophisticated way than simply starting and stopping them. It enables you to modify their behavior on the fly, which can be particularly useful if you need to adjust various settings during the execution of a long-running task. 

## tldr 
 
> Send input to a task.
> More information: <https://github.com/Nukesor/pueue>.

- Send input to a running command:

`pueue send {{task_id}} "{{input}}"`

- Send confirmation to a task expecting y/N (e.g. apt, cp):

`pueue send {{task_id}} {{y}}`
