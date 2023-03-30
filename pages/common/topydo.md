# topydo 
## chatgpt 
As an AI language model, I am not aware of any specific command named "topydo". It may be a custom or proprietary command specific to a particular system or application. Therefore, can you please provide more information about the context in which you came across this command, like the operating system or application where it is used? With this information, I can try to provide you with a detailed explanation of the topydo command. 

## tldr 
 
> A to-do list application that uses the todo.txt format.
> More information: <https://github.com/topydo/topydo>.

- Add a to-do to a specific project with a given context:

`topydo add "{{todo_message}} +{{project_name}} @{{context_name}}"`

- Add a to-do with a due date of tomorrow with a priority of `A`:

`topydo add "(A) {{todo _message}} due:{{1d}}"`

- Add a to-do with a due date of Friday:

`topydo add "{{todo_message}} due:{{fri}}"`

- Add a non-strict repeating to-do (next due = now + rec):

`topydo add "water flowers due:{{mon}} rec:{{1w}}"`

- Add a strict repeating to-do (next due = current due + rec):

`topydo add "{{todo_message}} due:{{2020-01-01}} rec:{{+1m}}"`

- Revert the last `topydo` command executed:

`topydo revert`
