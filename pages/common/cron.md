# cron 
## chatgpt 
Cron is a command used in Linux and Unix operating systems that allows users to schedule commands or scripts to run automatically at specified intervals. It is commonly used to automate repetitive tasks, such as system maintenance, backups, and updates.

Cron uses a configuration file called crontab to set up scheduled tasks. The crontab file contains a list of commands or scripts, along with the time intervals at which they should be executed.

To edit the crontab file, you can use the command "crontab -e". This will open the file in a text editor, where you can add or modify the scheduled tasks. Each line in the crontab file represents a single scheduled task, and includes the time interval and the command to be executed.

Cron uses a flexible syntax to specify time intervals, allowing users to specify precise times, specific days of the week or month, or more complex combinations. The syntax is as follows:

*     *     *     *     *  command to be executed
-     -     -     -     -
|     |     |     |     |
|     |     |     |     +----- day of the week (0 - 6) (Sunday = 0)
|     |     |     +---------- month (1 - 12)
|     |     +--------------- day of the month (1 - 31)
|     +-------------------- hour (0 - 23)
+------------------------- minute (0 - 59)

The fields are separated by spaces or tabs, and the asterisk (*) represents any value. For example, "* * * * * command" would execute the command every minute.

Once you have saved your changes to the crontab file, Cron will automatically run the scheduled tasks at the specified intervals. You can view the current list of scheduled tasks using the command "crontab -l". 

## tldr 
 
> `cron` is a system scheduler for running jobs or tasks unattended.
> The command to submit, edit or delete entries to `cron` is called `crontab`.

- View documentation for the original command:

`tldr crontab`
