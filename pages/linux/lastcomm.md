# lastcomm 
## chatgpt 
The "lastcomm" command is used in Linux or Unix systems to display information about the previously executed commands. When a user executes a command on the system, this command stores the information about the command in the /var/log/account/pacct file. The information stored includes the command name, the user who executes the command, the start time of execution, and the resources used during execution. 

The "lastcomm" command reads this file and displays the information about the recently executed commands. By default, the "lastcomm" command displays the command name, user name, type (whether it was a regular command or a system call), the start time, and the resources used during execution, but the output can be customized by using options.

Some common options used with the "lastcomm" command are:

- "-f" or "--fulltime": displays the full date and time of command execution.
- "-u" or "--user": specifies the user for which the command information is to be displayed.
- "-t" or "--time": specifies the time range for which the command information is to be displayed.
- "-S" or "--size": displays the amount of data transferred during execution.

For example, the command "lastcomm -u john" will display the information about the commands executed by the user "john", while "lastcomm -t today" will display the information about the commands executed today. 

## tldr 
 
> Show last commands executed.
> More information: <https://manpages.debian.org/stable/acct/lastcomm.1.en.html>.

- Print information about all the commands in the acct (record file):

`lastcomm`

- Display commands executed by a given user:

`lastcomm --user {{user}}`

- Display information about a given command executed on the system:

`lastcomm --command {{command}}`

- Display information about commands executed on a given terminal:

`lastcomm --tty {{terminal_name}}`
