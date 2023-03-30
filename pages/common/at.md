# at 
## chatgpt 
The "at" command in Linux and Unix-based operating systems schedules a task to be executed at a specified time. The syntax for this command is as follows:

at [-r] [-f file] [-mldbv] TIME

- [-r]: Cancels a previously scheduled task.
- [-f file]: Specifies the file containing the shell command to be executed.
- [-mldbv]: Sets the mail options.
- TIME: Specifies the time at which the command should be executed. The format for this can be either a specific time (e.g. "10:30pm"), or a time relative to the current time (e.g. "+5 minutes").

Here's an example of using the "at" command:

```
$ at 11:00pm
at> /usr/local/bin/backup.sh
at> <EOT>
```

This command will execute the "backup.sh" script located in "/usr/local/bin" at 11:00pm. The "<EOT>" symbol is used to indicate the end of the command, which is necessary when entering multi-line commands. Upon successful execution, the output of the command will be sent to the user's email. The default email address is the user's login name on the local machine. 

## tldr 
 
> Execute commands once at a later time.
> Service atd (or atrun) should be running for the actual executions.
> More information: <https://manned.org/at>.

- Execute commands from standard input in 5 minutes (press `Ctrl + D` when done):

`at now + 5 minutes`

- Execute a command from standard input at 10:00 AM today:

`echo "{{./make_db_backup.sh}}" | at 1000`

- Execute commands from a given file next Tuesday:

`at -f {{path/to/file}} 9:30 PM Tue`
