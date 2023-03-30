# runit 
## chatgpt 
The command "runit" is a Unix utility that is used to supervise and manage system services. It is typically used as a replacement for the traditional SysV init system or systemd. Runit is designed to be simple, efficient and reliable, so that it can be easily used in embedded systems or on servers where uptime is critical.

When you run the "runit" command, it starts the runit service management daemon. This daemon is responsible for starting and stopping services, and monitoring their status. It reads configuration files located in various directories to determine which services should be started or stopped.

Here are some common actions you can perform with the "runit" command:

- Starting a service: You can start a service by running the "sv start" command followed by the name of the service. For example, to start the "httpd" service, you would run "sv start httpd".
- Stopping a service: You can stop a service by running the "sv stop" command followed by the name of the service. For example, to stop the "httpd" service, you would run "sv stop httpd".
- Restarting a service: You can restart a service by running the "sv restart" command followed by the name of the service. For example, to restart the "httpd" service, you would run "sv restart httpd".
- Checking the status of a service: You can check the status of a service by running the "sv status" command followed by the name of the service. For example, to check the status of the "httpd" service, you would run "sv status httpd".

Overall, the "runit" command is an essential tool for managing system services in Unix environments, and it provides a reliable, efficient and simple way to manage services on servers and embedded systems. 

## tldr 
 
> 3-stage init system.
> More information: <http://smarden.org/runit/runit.8.html>.

- Start runit's 3-stage init scheme:

`runit`

- Shut down runit:

`kill --CONT {{runit_pid}}`
