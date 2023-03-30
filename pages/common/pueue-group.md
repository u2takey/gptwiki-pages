# pueue group 
## chatgpt 
The command "pueue group" is used in the task management tool called "pueue" to group tasks into specific categories. This can be useful for organizing tasks based on their purpose, project, or priority.

When you run the "pueue group" command, it will prompt you to enter the name of the group you want to create. Once you've entered the group name, you can add tasks to that group using the "pueue add" command and specifying the group with the "-g" flag.

For example, let's say you want to create a group called "Important Tasks" and add a task to that group called "Finish report":

1. Run the command "pueue group" and enter "Important Tasks" as the group name.
2. Run the command "pueue add --group 'Important Tasks' 'Finish report'" to add the task to the group.
3. You can then view all tasks in the "Important Tasks" group by running the command "pueue ls --group 'Important Tasks'".

In summary, the "pueue group" command allows you to create and manage groups of tasks in the pueue task management tool. 

## tldr 
 
> Display, add or remove groups.
> More information: <https://github.com/Nukesor/pueue>.

- Show all groups with their statuses and number of parallel jobs:

`pueue group`

- Add a custom group:

`pueue group --add "{{group_name}}"`

- Remove a group and move its tasks to the default group:

`pueue group --remove "{{group_name}}"`
