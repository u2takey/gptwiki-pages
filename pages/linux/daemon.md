# daemon 
## chatgpt 
The command "daemon" is not a specific command in most operating systems, but generally refers to a process that runs in the background, continuously and independently from the user interface or controlling terminal. A daemon is typically responsible for providing some system service or functionality, such as network services or automatic backups.

Different systems have different ways of starting, stopping or controlling daemons, but some common methods include running the daemon as a system service, using a process manager like systemd, init or launchd, or simply running the command in the background with a nohup or & option.

Overall, the "daemon" command can refer to any kind of long-running background process that provides a specific system function or service. 

## tldr 
 
> Run processes into daemons.
> More information: <https://manned.org/man/daemon.1>.

- Run a command as a daemon:

`daemon --name="{{name}}" {{command}}`

- Run a command as a daemon which will restart if the command crashes:

`daemon --name="{{name}}" --respawn {{command}}`

- Run a command as a daemon which will restart if it crashes, with two attempts every 10 seconds:

`daemon --name="{{name}}" --respawn --attempts=2 --delay=10 {{command}}`

- Run a command as a daemon, writing logs to a specific file:

`daemon --name="{{name}}" --errlog={{path/to/file.log}} {{command}}`

- Kill a daemon (SIGTERM):

`daemon --name="{{name}}" --stop`

- List daemons:

`daemon --list`
