# task 
## chatgpt 
The command "task" is a built-in command in some operating systems such as Linux and Windows. It is a utility that allows users to manage and monitor tasks or processes running on the system.

When executed, the "task" command provides a list of all the tasks and their details, such as the process ID, name, memory usage, priority, and status. The output is usually displayed in the terminal window.

The "task" command also provides several options to perform tasks such as terminating or killing a task, changing the priority of a task, and displaying detailed information about a specific task.

For example, to terminate a task with a specific process ID, the command syntax would be "taskkill /PID [process ID] /F". The "/PID" option specifies the process ID of the task to be terminated, and the "/F" option forces the task to be terminated without prompting for confirmation.

Overall, the "task" command is a useful tool for users who need to manage and monitor tasks on their systems. 

## tldr 
 
> Command-line to-do list manager.
> More information: <https://taskwarrior.org/docs/>.

- Add a new task which is due tomorrow:

`task add {{description}} due:{{tomorrow}}`

- Update a task's priority:

`task {{task_id}} modify priority:{{H|M|L}}`

- Complete a task:

`task {{task_id}} done`

- Delete a task:

`task {{task_id}} delete`

- List all open tasks:

`task list`

- List open tasks due before the end of the week:

`task list due.before:{{eow}}`

- Show a graphical burndown chart, by day:

`task burndown.daily`

- List all reports:

`task reports`
