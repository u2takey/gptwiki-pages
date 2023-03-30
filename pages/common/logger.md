# logger 
## chatgpt 
The logger command is a system logging utility in Unix-based operating systems that enables messages to be sent to the system log, or to a specific file. 

The command syntax for logger is as follows:

logger [OPTIONS] [MESSAGE]

Where OPTIONS are various flags which can be used to modify the behavior of the command, and MESSAGE is the actual message to be logged. 

Some of the most commonly used options for logger are:

- -p : Specifies the logging priority level. Priority levels range from 0 (emergency) to 7 (debug).
- -t : Sets the tag or identifier associated with the message.
- -s : Logs the message to standard error instead of the system log.

The MESSAGE argument can be anything that the user wants to log. This can include simple text, variables, or output from other commands. 

The logger command is very useful for system administrators and developers who need to keep track of activity on a system or debug issues. By logging messages, they can easily trace back events that occurred and determine the cause of problems. 

## tldr 
 
> Add messages to syslog (/var/log/syslog).
> More information: <https://manned.org/logger>.

- Log a message to syslog:

`logger {{message}}`

- Take input from `stdin` and log to syslog:

`echo {{log_entry}} | logger`

- Send the output to a remote syslog server running at a given port. Default port is 514:

`echo {{log_entry}} | logger --server {{hostname}} --port {{port}}`

- Use a specific tag for every line logged. Default is the name of logged in user:

`echo {{log_entry}} | logger --tag {{tag}}`

- Log messages with a given priority. Default is `user.notice`. See `man logger` for all priority options:

`echo {{log_entry}} | logger --priority {{user.warning}}`
