# openrc 
## chatgpt 
The "openrc" command is used to start or stop OpenRC, which is a dependency-based init system used by certain Linux distributions, such as Gentoo and Alpine Linux. 

Init systems are the first processes started by the kernel during boot, and they are responsible for bringing up the entire system by running various services and daemons. OpenRC is designed to be lightweight, fast, and flexible, and it works by using shell scripts and configuration files to define which services should be started or stopped, and in which order. 

The following are some common usage of the "openrc" command:
- sudo openrc - Starts the OpenRC init system.
- sudo openrc-stop - Stops the OpenRC init system.
- sudo openrc-restart - Restarts the OpenRC init system.
- sudo openrc-status - Displays the status of all configured services and daemons.

Overall, the "openrc" command is a crucial tool for managing the OpenRC init system on a Linux system, allowing users to start, stop, and monitor the various services and daemons that are required for the system to function properly. 

## tldr 
 
> The OpenRC service manager.
> See also `rc-status`, `rc-update`, and `rc-service`.
> More information: <https://wiki.gentoo.org/wiki/OpenRC>.

- Change to a specific runlevel:

`sudo openrc {{runlevel_name}}`

- Change to a specific runlevel, but don't stop any existing services:

`sudo openrc --no-stop {{runlevel_name}}`
