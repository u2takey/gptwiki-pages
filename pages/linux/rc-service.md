# rc-service 
## chatgpt 
rc-service is a command that is used in Unix-based operating systems, such as Linux, to manage services on the system. It is a part of the OpenRC init system, which is used as an alternative to systemd in some distributions.

The command is typically used to start, stop, and manage the behavior of system services. Each service on the system is represented as a script file in the /etc/init.d/ directory. The rc-service command operates by running these scripts to start or stop a service.

The basic syntax of the command is:

```
rc-service <service-name> <command>
```

The service-name is the name of the service that you want to manage, and the command is the action that you want to perform on the service. Some of the commonly used commands are:

- start: Start a service
- stop: Stop a service
- restart: Restart a service
- status: Get the status of a service
- enable: Configure a service to start automatically at boot time.
- disable: Remove a service from the list of services that start automatically at boot time.

For example, to start the Apache web server on a Linux system that uses OpenRC, you would use the following command:

```
rc-service apache2 start
```

This runs the script file in /etc/init.d/apache2 to start the Apache service.

Overall, the rc-service command is a useful tool for managing system services on Unix-based systems that use the OpenRC init system. 

## tldr 
 
> Locate and run OpenRC services with arguments.
> See also `openrc`.
> More information: <https://manned.org/rc-service>.

- Show a service's status:

`rc-service {{service_name}} status`

- Start a service:

`sudo rc-service {{service_name}} start`

- Stop a service:

`sudo rc-service {{service_name}} stop`

- Restart a service:

`sudo rc-service {{service_name}} restart`

- Simulate running a service's custom command:

`sudo rc-service --dry-run {{service_name}} {{command_name}}`

- Actually run a service's custom command:

`sudo rc-service {{service_name}} {{command_name}}`

- Resolve the location of a service definition on disk:

`sudo rc-service --resolve {{service_name}}`
