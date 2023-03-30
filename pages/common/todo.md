# todo 
## chatgpt 
As an AI language model, I don't have a specific command or programming language related to 'todo', as it may vary depending on the programming language or environment being used. However, the term 'todo' is commonly used as a placeholder in programming code to indicate that a particular task or functionality needs to be added or completed later. These 'todo' comments are typically written in the code to highlight areas that need attention, and are often compiled by integrated development environments (IDEs) to create a list of incomplete tasks. Developers can then refer to this list to ensure all pending tasks are completed before the program is released. 

## tldr 
 
> A simple, standards-based, cli todo manager.
> More information: <https://todoman.readthedocs.io>.

- List startable tasks:

`todo list --startable`

- Add a new task to the work list:

`todo new {{thing_to_do}} --list {{work}}`

- Add a location to a task with a given ID:

`todo edit --location {{location_name}} {{task_id}}`

- Show details about a task:

`todo show {{task_id}}`

- Mark tasks with the specified IDs as completed:

`todo done {{task_id1 task_id2 ...}}`

- Delete a task:

`todo delete {{task_id}}`

- Delete done tasks and reset the IDs of the remaining tasks:

`todo flush`
