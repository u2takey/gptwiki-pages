# chkconfig 
## chatgpt 
The `chkconfig` command is a Linux utility that is used to manage the runlevel configuration of system services. It can be used to enable or disable services to start automatically during the system boot process.

Here's a breakdown of the `chkconfig` command:

Syntax:
```
chkconfig [options] <service> <on/off>
```

Options:
- `--add`: Adds a new service to the system.
- `--del`: Deletes an existing service from the system.
- `--list`: Lists all services and their current status.
- `--level <runlevel>`: Specifies the runlevel to modify.
- `--help`: Displays help and usage information.

Usage:
- `chkconfig <service>`: Displays the current status of a service.
- `chkconfig <service> on`: Enables a service to start automatically at boot time.
- `chkconfig <service> off`: Disables a service from starting automatically at boot time.

For example, to enable the Apache web server service to start automatically on system boot, we would run the following command:
```
chkconfig httpd on
```

This tells the `chkconfig` utility to enable the `httpd` service to start automatically in all runlevels. Similarly, to disable the service from starting automatically on boot, we would use:
```
chkconfig httpd off
```

This removes the `httpd` service from the list of services that start automatically during system boot. 

## tldr 
 
> Manage the runlevel of services on CentOS 6.
> More information: <https://manned.org/chkconfig>.

- List services with runlevel:

`chkconfig --list`

- Show a service's runlevel:

`chkconfig --list {{ntpd}}`

- Enable service at boot:

`chkconfig {{sshd}} on`

- Enable service at boot for runlevels 2, 3, 4, and 5:

`chkconfig --level {{2345}} {{sshd}} on`

- Disable service at boot:

`chkconfig {{ntpd}} off`

- Disable service at boot for runlevel 3:

`chkconfig --level {{3}} {{ntpd}} off`
