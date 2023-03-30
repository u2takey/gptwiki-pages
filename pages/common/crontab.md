# crontab 
## chatgpt 
Crontab is a command used in Unix-based operating systems (such as Linux) to manage scheduled tasks. It allows users to schedule automated tasks, such as running a script or command at a specified interval.

Here are a few key details about the crontab command:

- The crontab command is used to edit, view, and manage the crontab file for a user. The crontab file contains a list of commands to be executed at specified times and intervals.
- The syntax for the crontab command is as follows: crontab [option] [filename]. The options available include -e (edit the crontab file), -l (list the user's crontab file), and -r (remove the user's crontab file).
- The crontab file is organized into six fields, each representing a different aspect of the schedule. The fields are separated by a space or tab, and are ordered as follows: minute, hour, day of month, month, day of week, command.
- Asterisks (*) are used as wildcards in the crontab file to represent all possible values for a field. For example, * in the hour field would mean "every hour".
- To set a specific value for a field, simply enter that value. For example, "0" in the minute field would specify the task should run at the top of the hour.
- Ranges can be specified using a hyphen (-). For example, "1-5" in the day of week field would mean "Monday through Friday".
- Multiple values can be specified using a comma (,). For example, "1,15,30,45" in the minute field would mean "run the task at 1, 15, 30, and 45 minutes past the hour".
- Comments can be added to the crontab file using the pound sign (#), which will ignore the rest of the line. 

Overall, the crontab command is a powerful tool for scheduling automated tasks in a Unix-based operating system. With a little practice, users can easily create and manage custom schedules for their specific needs. 

## tldr 
 
> Schedule cron jobs to run on a time interval for the current user.
> More information: <https://crontab.guru/>.

- Edit the crontab file for the current user:

`crontab -e`

- Edit the crontab file for a specific user:

`sudo crontab -e -u {{user}}`

- Replace the current crontab with the contents of the given file:

`crontab {{path/to/file}}`

- View a list of existing cron jobs for current user:

`crontab -l`

- Remove all cron jobs for the current user:

`crontab -r`

- Sample job which runs at 10:00 every day (* means any value):

`0 10 * * * {{command_to_execute}}`

- Sample crontab entry, which runs a command every 10 minutes:

`*/10 * * * * {{command_to_execute}}`

- Sample crontab entry, which runs a certain script at 02:30 every Friday:

`30 2 * * Fri {{/absolute/path/to/script.sh}}`
