# systemctl 
## chatgpt 
Systemctl is a command-line utility in Linux systems that controls and manages the system's services and daemons. It is a part of the Systemd system management daemon, which is a replacement for the traditional SysV init system.

With systemctl, you can view the status of services, start, stop, enable or disable services, reload configuration files, and more. It is used to manage the system services and processes running on Linux operating systems.

Some of the commonly used systemctl commands are:

1. systemctl status <service> - Displays the current status of a service.
2. systemctl start <service> - Starts a service.
3. systemctl stop <service> - Stops a service.
4. systemctl enable <service> - Enables a service to start automatically on system boot.
5. systemctl disable <service> - Disables a service from starting automatically on system boot.
6. systemctl restart <service> - Restarts a service.
7. systemctl reload <service> - Reloads the configuration of a service.


In summary, systemctl is a powerful command-line utility that is used to control and manage the system's services and daemons efficiently. It can help system administrators with tasks such as troubleshooting, debugging, and managing the system services. 

## tldr 
 
> Control the systemd system and service manager.
> More information: <https://www.freedesktop.org/software/systemd/man/systemctl.html>.

- Show all running services:

`systemctl status`

- List failed units:

`systemctl --failed`

- Start/Stop/Restart/Reload a service:

`systemctl {{start|stop|restart|reload}} {{unit}}`

- Show the status of a unit:

`systemctl status {{unit}}`

- Enable/Disable a unit to be started on bootup:

`systemctl {{enable|disable}} {{unit}}`

- Mask/Unmask a unit to prevent enablement and manual activation:

`systemctl {{mask|unmask}} {{unit}}`

- Reload systemd, scanning for new or changed units:

`systemctl daemon-reload`

- Check if a unit is enabled:

`systemctl is-enabled {{unit}}`
