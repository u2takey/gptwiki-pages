# pueue parallel 
## chatgpt 
The command "pueue parallel" is used to run multiple commands or tasks in parallel using the Pueue task manager. 

Here's a breakdown of the components of the command:

- "pueue" - this is the name of the task manager tool that will be used to execute the command(s). Pueue stands for "Processing in a queue", and it is a command-line tool that allows users to manage and run tasks in the background. 

- "parallel" - this is an argument or option that is passed to the Pueue tool, indicating that the commands to be executed should be run in parallel. 

When you run the "pueue parallel" command, you will be prompted to enter the commands you want to execute in parallel. You can enter multiple commands, each separated by a comma, and Pueue will schedule them to run concurrently. 

For example, if you enter the following command after running "pueue parallel": 

```
$ echo "Task 1", echo "Task 2", echo "Task 3"
```

Pueue will run three tasks in parallel, each of which will output a different message to the console: 

```
Task 1
Task 2
Task 3
```

Overall, using the "pueue parallel" command with the Pueue tool is a useful way to manage and run multiple tasks at once, improving efficiency and productivity. 

## tldr 
 
> Set the amount of allowed parallel tasks.
> More information: <https://github.com/Nukesor/pueue>.

- Set the maximum number of tasks allowed to run in parallel, in the default group:

`pueue parallel {{max_number_of_parallel_tasks}}`

- Set the maximum number of tasks allowed to run in parallel, in a specific group:

`pueue parallel --group {{group_name}} {{maximum_number_of_parallel_tasks}}`
