# reboot 
## chatgpt 
The command "reboot" is used in Unix-like operating systems to initiate a system reboot. When issued, the command causes the operating system to shut down all running processes, unmount all file systems, and then perform a hard reset of the system. 

This command is typically only used when there is a problem with the system that requires a reboot in order to fix it. There are several ways to initiate a reboot on Unix-like systems, but the "reboot" command is one of the simplest and most direct.

When executing the "reboot" command, the system will prompt the user with a message asking for confirmation before initiating the reboot. This is to prevent accidental reboots and give the user a chance to save any important work before the system is shut down.

It's worth noting that the "reboot" command should be used with caution, as it can cause the loss of unsaved data and potentially harm the system if used improperly. It's always best to save any important work before issuing this command and to use it only when necessary. 

## tldr 
 
> Reboot the system.
> More information: <https://manned.org/reboot.8>.

- Reboot the system:

`reboot`

- Power off the system (same as `poweroff`):

`reboot --poweroff`

- Halt the system (same as `halt`):

`reboot --halt`

- Reboot immediately without contacting the system manager:

`reboot --force`

- Write the wtmp shutdown entry without rebooting the system:

`reboot --wtmp-only`
