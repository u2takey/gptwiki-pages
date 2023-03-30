# todoist 
## chatgpt 
As an AI language model, I can give you the definition of the task manager app Todoist.

Todoist is a digital task manager that helps people organize and prioritize their work and personal tasks. The app allows users to create to-do lists, set reminders, and collaborate with others on tasks. It can be used on a variety of devices like smartphones, tablets, and computers. The app offers various features such as categorizing tasks by projects, adding tags, assigning priority levels, and creating recurring tasks. Additionally, Todoist integrates with various tools like Slack, Gmail, and Google Calendar, making it easier for users to manage their tasks and stay organized. Overall, Todoist is a versatile and easy-to-use digital task manager that helps people stay on top of their to-do lists and increase productivity. 

## tldr 
 
> Access Todoist from the command-line.
> More information: <https://github.com/sachaos/todoist>.

- Add a task:

`todoist add "{{task_name}}"`

- Add a high priority task with a label, project, and due date:

`todoist add "{{task_name}}" --priority {{1}} --label-ids "{{label_id}}" --project-name "{{project_name}}" --date "{{tmr 9am}}"`

- Add a high priority task with a label, project, and due date in quick mode:

`todoist quick '#{{project_name}} "{{tmr 9am}}" p{{1}} {{task_name}} @{{label_name}}'`

- List all tasks with a header and color:

`todoist --header --color list`

- List all high priority tasks:

`todoist list --filter p{{1}}`

- List today's tasks with high priority that have the specified label:

`todoist list --filter '(@{{label_name}} | {{today}}) & p{{1}}'`
