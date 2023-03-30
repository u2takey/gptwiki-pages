# supervisord 
## chatgpt 
Supervisord is a process control system that is designed to monitor and manage other processes on a Linux or Unix-like system. 

When you run the ‘supervisord’ command, it starts the supervisord daemon, which then reads its configuration file and starts the process as specified in the configuration. 

The configuration file can be located at /etc/supervisor/supervisord.conf or /etc/supervisord.conf. This file contains information about the processes that supervisord should start and manage, and how to manage them. 

Overall, the ‘supervisord’ command is used to start the supervisord process control system and load the configuration file for managing other processes. 

## tldr 
 
> Supervisor is a client/server system for controlling some processes on UNIX-like operating systems.
> Supervisord is the server part of supervisor; it is primarily managed via a configuration file.
> More information: <http://supervisord.org>.

- Start supervisord with specified configuration file:

`supervisord -c {{path/to/file}}`

- Run supervisord in the foreground:

`supervisord -n`
