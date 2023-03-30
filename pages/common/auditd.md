# auditd 
## chatgpt 
The `auditd` command launches the `auditd` daemon which is responsible for generating and storing audit records in the system. The auditd daemon is a part of the audit framework which is used to monitor and record activities occurring within the system. 

When `auditd` is started, it reads the configuration file `/etc/audit/auditd.conf` to determine the rules for generating audit records. These rules are defined in terms of events and actions, where an event is a system call or a file access, and an action is the response taken when an event occurs. The audit records are stored in binary format in the `/var/log/audit/` directory.

Audit records allow system administrators to track the activities of users and processes on the system, and can be used for security and compliance purposes. The audit system can be configured to monitor specific activities, such as file access or system calls, and can generate alerts or notifications when suspicious activity is detected.

Overall, the `auditd` command is a critical tool for enhancing the security and auditability of a system by providing an automated and comprehensive audit trail of the activities occurring within the system. 

## tldr 
 
> This responds to requests from the audit utility and notifications from the kernel.
> It should not be invoked manually.
> More information: <https://manned.org/auditd>.

- Start the daemon:

`auditd`

- Start the daemon in debug mode:

`auditd -d`

- Start the daemon on-demand from launchd:

`auditd -l`
