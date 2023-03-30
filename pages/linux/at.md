# at 
## chatgpt 
The `at` command is a command-line utility used in Linux and Unix systems to schedule commands or scripts to run at a specified time in the future. It allows users to schedule a task to be executed at a specific time, either a one-time execution or a recurring task. 

The syntax of the `at` command is as follows: 

`at [-f filename] [-m] [-q queuename] [-t time] [time]`

The options for the `at` command are:

- `-f`: specifies the filename containing the commands to be executed

- `-m`: sends an email to the user when the job has completed

- `-q`: specifies the queue name to use. A higher priority queue means a job is executed sooner.

- `-t`: specifies the time format in which the job should be executed. 

- `time`: indicates when the job should be executed. This can be specified in various formats such as HH:MM, HH:MM AM or PM, or YYYY-MM-DD HH:MM.

Once the task has been scheduled, it can be edited or removed by using the `atrm` or `atq` commands.

Example: 

To schedule a task to run at 3PM on 15th August 2021, the command would be:

`at 3PM 15 Aug 21`

This would open a new prompt where we can enter the commands to be executed at that time. 

To specify the command to be executed from a file, use the `-f` option:

`at -f script.sh 3PM 15 Aug 21` 

This would execute the commands mentioned in the `script.sh` file at the specified time. 

## tldr 
 
> Executes commands at a specified time.
> More information: <https://man.archlinux.org/man/at.1>.

- Open an `at` prompt to create a new set of scheduled commands, press `Ctrl + D` to save and exit:

`at {{hh:mm}}`

- Execute the commands and email the result using a local mailing program such as Sendmail:

`at {{hh:mm}} -m`

- Execute a script at the given time:

`at {{hh:mm}} -f {{path/to/file}}`

- Display a system notification at 11pm on February 18th:

`echo "notify-send '{{Wake up!}}'" | at {{11pm}} {{Feb 18}}`
