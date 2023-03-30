# timetrap 
## chatgpt 
Timetrap is a command-line time tracking tool that allows you to keep track of how much time you spend on various tasks.

Here are some of the key features of Timetrap:

1. Simple interface: Timetrap has a simple and easy-to-use command-line interface, making it easy to start and stop time entries.

2. Flexible reporting: Timetrap allows you to generate custom reports based on different time periods, tags, projects, and more.

3. Multiple backends: Timetrap supports multiple backends for storage, including SQLite, YAML, and Active Record.

4. Extensive documentation: Timetrap has extensive documentation that covers all of its features and functionality.

Here are some of the common commands that you can use with Timetrap:

1. timetrap start <task name>: This command starts a new time entry for the specified task.

2. timetrap stop: This command stops the current time entry.

3. timetrap sheet: This command generates a report of all of your time entries.

4. timetrap report <options>: This command generates a custom report based on specified options.

5. timetrap edit <entry id>: This command allows you to edit a specific time entry.

Overall, Timetrap is a powerful and flexible time tracking tool that can help you stay organized and productive. 

## tldr 
 
> Simple command-line time tracker written in Ruby.
> More information: <https://github.com/samg/timetrap>.

- Create a new timesheet:

`timetrap sheet {{timesheet}}`

- Check in an entry started 5 minutes ago:

`timetrap in --at "{{5 minutes ago}}" {{entry_notes}}`

- Display the current timesheet:

`timetrap display`
