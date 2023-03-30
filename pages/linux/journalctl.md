# journalctl 
## chatgpt 
journalctl is a command in Linux-based systems that is used to access and display the contents of the systemd log files. It allows the user to view and analyze system journal logs maintained by the syslog daemon and systemd system and service manager.

The journalctl command enables the user to query the system log data for specific information such as types of messages, time range, specific units, priority level, etc. It also provides various filtering options to search for specific events or patterns of messages.

The basic syntax of the journalctl command can be used to display the entire system log history, in reverse chronological order. This is done by simply entering the command “journalctl” in the terminal. 

Some of the commonly used options with the journalctl command include:

- -u : This option allows the user to filter the logs based on specific service/unit names.
- -p : This option enables the user to filter the logs based on a specific priority level. 
- -f : This option allows the user to view the log in real-time, i.e., follow the log in a continuously updating view. 
- --since/-S, --until/-U : These options allow the user to filter the logs based on a specific time frame between the specified date and time range. 
- -o : This option allows the user to specify the output format of the logs, such as JSON, plain text, or pretty-printed output.
- --boot/-b : This option allows the user to view the logs for a specific boot sequence.


In summary, the journalctl command is a powerful tool for accessing and analyzing the system logs on Linux-based systems. It allows the user to search and filter logs based on various criteria to help in troubleshooting issues, identifying potential security threats, or analyzing system performance. 

## tldr 
 
> Query the systemd journal.
> More information: <https://manned.org/journalctl>.

- Show all messages with priority level 3 (errors) from this [b]oot:

`journalctl -b --priority={{3}}`

- Show all messages from last [b]oot:

`journalctl -b -1`

- Delete journal logs which are older than 2 days:

`journalctl --vacuum-time={{2d}}`

- [f]ollow new messages (like `tail -f` for traditional syslog):

`journalctl -f`

- Show all messages by a specific [u]nit:

`journalctl -u {{unit}}`

- Filter messages within a time range (either timestamp or placeholders like "yesterday"):

`journalctl --since {{now|today|yesterday|tomorrow}} --until {{YYYY-MM-DD HH:MM:SS}}`

- Show all messages by a specific process:

`journalctl _PID={{pid}}`

- Show all messages by a specific executable:

`journalctl {{path/to/executable}}`
