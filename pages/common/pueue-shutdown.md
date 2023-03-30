# pueue shutdown 
## chatgpt 
The command "pueue shutdown" can refer to different tools depending on the context, but assuming pueue refers to Pueue Task Manager, a command-line task manager for managing long-running shell commands, then "pueue shutdown" refers to a command that shuts down the Pueue daemon, stopping all running tasks and clearing the waiting queue. 

This command is used when you want to stop all the running tasks and close the Pueue daemon gracefully. If you don't shut down the daemon, it may keep running in the background, consuming system resources.

When you execute "pueue shutdown" command, it will send a termination signal to all running tasks, which will immediately stop them. Then, it will remove any tasks queued and cancel any tasks that haven't started running yet. Finally, it will close the daemon gracefully, leaving no running processes in the background. 

It is recommended to use this command to close Pueue daemon rather than killing it through the system monitor or interrupting it with Ctrl+C, as those methods may leave tasks running or cause other issues.

Note that when you restart Pueue, you will need to re-queue any tasks that were removed during the shutdown process. 

## tldr 
 
> Remotely shut down the daemon.
> Only use this subcommand if the daemon isn't started by a service manager.
> More information: <https://github.com/Nukesor/pueue>.

- Shutdown the daemon without a service manager:

`pueue shutdown`
