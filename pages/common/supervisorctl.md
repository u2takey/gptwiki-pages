# supervisorctl 
## chatgpt 
Supervisorctl is a command-line tool that is used to manage processes that are controlled by the Supervisor process control system. The Supervisor process control system is a client/server system that allows users to monitor and control processes on a Unix-based operating system.

The supervisorctl command is used to start, stop, restart, and monitor processes that are controlled by the Supervisor process control system. When you execute the supervisorctl command, you are launching a command-line interface that enables you to interact with the Supervisor daemon and perform actions on the processes it manages.

Some of the common actions that you can perform with the supervisorctl command include:

1. Starting a process: This action launches a process that is managed by the Supervisor process control system. To start a process, you can use the following command:

   supervisorctl start process_name

2. Stopping a process: This action halts the execution of the process that is managed by the Supervisor process control system. To stop a process, you can use the following command:

   supervisorctl stop process_name

3. Restarting a process: This action stops a process and then starts it again. To restart a process, you can use the following command:

   supervisorctl restart process_name

4. Checking the status of a process: This action displays the current status of a process that is managed by the Supervisor process control system. To check the status of a process, you can use the following command:

   supervisorctl status process_name

These are just a few examples of the actions that can be performed with the supervisorctl command. The supervisorctl command is a powerful tool that can be used to manage a wide range of processes on a Unix-based operating system. 

## tldr 
 
> Supervisor is a client/server system that allows its users to control a number of processes on UNIX-like operating systems.
> Supervisorctl is the command-line client piece of the supervisor which provides a shell-like interface.
> More information: <http://supervisord.org>.

- Start/stop/restart a process:

`supervisorctl {{start|stop|restart}} {{process_name}}`

- Start/stop/restart all processes in a group:

`supervisorctl {{start|stop|restart}} {{group_name}}:*`

- Show last 100 **bytes** of process `stderr`:

`supervisorctl tail -100 {{process_name}} stderr`

- Keep displaying `stdout` of a process:

`supervisorctl tail -f {{process_name}} stdout`

- Reload process config file to add/remove processes as necessary:

`supervisorctl update`
