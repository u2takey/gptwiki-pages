# service 
## chatgpt 
The "service" command is used in Linux to manage and control system services. 

When using the "service" command, the first parameter should be the name of the service you want to manage. This name usually corresponds to the name of the package that installed the service, and can be found in the "/etc/init.d" directory. 

Once you have specified the service name, you can then use various options to start, stop, restart, or check the status of the service. For example: 

- "service apache2 start" would start the "apache2" service if it is not already running
- "service ssh restart" would restart the "ssh" service 
- "service mysql status" would check the status of the "mysql" service 

The specific available options for each service may vary depending on how it was configured, but typically include "start", "stop", "restart", "status", and possibly others. 

Overall, the "service" command provides an easy and standardized way to manage and maintain system services on a Linux machine. 

## tldr 
 
> Manage services by running init scripts.
> The full script path should be omitted (`/etc/init.d/` is assumed).
> More information: <https://manned.org/service>.

- List the name and status of all services:

`service --status-all`

- Start/Stop/Restart/Reload service (start/stop should always be available):

`service {{service_name}} {{start|stop|restart|reload}}`

- Do a full restart (runs script twice with start and stop):

`service {{service_name}} --full-restart`

- Show the current status of a service:

`service {{service_name}} status`
