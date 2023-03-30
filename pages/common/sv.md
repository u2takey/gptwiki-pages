# sv 
## chatgpt 
The command "sv" is a shorthand for "supervise" and is typically used in Unix and Unix-like operating systems. It is a part of the runit service management system available in these operating systems. The "sv" command is used to manage system services that are managed by runit.

There are various options that can be used with the "sv" command to perform different operations on a given service. Some of the commonly used options are:

- sv start <service-name>: This option is used to start a specified service.
- sv stop <service-name>: This option is used to stop a specified service.
- sv status <service-name>: This option is used to check the status of a specified service.
- sv restart <service-name>: This option is used to restart a specified service.
- sv enable <service-name>: This option is used to enable a specified service so that it starts automatically during system boot.
- sv disable <service-name>: This option is used to disable a specified service so that it does not start automatically during system boot.

In general, the "sv" command is very useful for system administrators who need to manage services running on a Unix or Unix-like operating system. It provides a simple and efficient way to manage service processes and ensure that they are running smoothly. 

## tldr 
 
> Control a running runsv service.
> More information: <https://manpages.ubuntu.com/manpages/latest/man8/sv.8.html>.

- Start a service:

`sudo sv up {{path/to/service}}`

- Stop a service:

`sudo sv down {{path/to/service}}`

- Get service status:

`sudo sv status {{path/to/service}}`

- Reload a service:

`sudo sv reload {{path/to/service}}`

- Start a service, but only if it's not running and don't restart it if it stops:

`sudo sv once {{path/to/service}}`
