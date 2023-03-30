# rc-status 
## chatgpt 
The "rc-status" command is typically used in Linux systems to display the current status of the services that are managed by the "rc" subsystem, which is responsible for starting, stopping, and managing essential system services during the boot process.

When you run the "rc-status" command, it will display a table that lists all the runlevels in the system, along with the status of each service that's associated with that runlevel. The status of each service can be one of several values, including "stopped", "started", "on demand", "error", or "disabled".

Here's an example output of the "rc-status" command:

```
Runlevel: default
 dbus            [ started  ]
 docker          [ started  ]
 elasticsearch   [ started  ]
 kibana          [ started  ]
 logstash        [ started  ]
 nginx           [ started  ]
 redis           [ started  ]
 sshd            [ started  ]
 syslog-ng      [ started  ]
 unbound         [ started  ]
```

This output shows that all the services associated with the "default" runlevel are currently started and running. The square brackets around the status of each service indicate that they've been started by the "rc" subsystem.

In summary, the "rc-status" command is a useful tool for checking the status of system services managed by the "rc" subsystem in Linux systems. It provides an overview of the services that are currently running, their statuses, and their associated runlevels. This information can be helpful in troubleshooting issues or optimizing system performance. 

## tldr 
 
> Show status info about runlevels.
> See also `openrc`.
> More information: <https://manned.org/rc-status>.

- Show a summary of services and their status:

`rc-status`

- Include services in all runlevels in the summary:

`rc-status --all`

- List services that have crashed:

`rc-status --crashed`

- List manually started services:

`rc-status --manual`

- List supervised services:

`rc-status --supervised`

- Get the current runlevel:

`rc-status --runlevel`

- List all runlevels:

`rc-status --list`
