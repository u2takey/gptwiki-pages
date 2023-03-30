# poweroff 
## chatgpt 
The `poweroff` command is used to shut down the computer or turn off the power. 

When executed, it sends a signal to the operating system to shut down all processes, close all open files, and flush any cached data to the storage devices. Once this process is complete, the computer hardware is instructed to turn off the power to the system.

Note that this command should be used with caution as it immediately shuts down and turns off power to the system without performing any further operations or checks. It is recommended to save any unsaved work before executing this command. 

## tldr 
 
> Power off the system.
> More information: <https://www.man7.org/linux/man-pages/man8/poweroff.8.html>.

- Power off the system:

`poweroff`

- Halt the system (same as `halt`):

`poweroff --halt`

- Reboot the system (same as `reboot`):

`poweroff --reboot`

- Shut down immediately without contacting the system manager:

`poweroff --force --force`

- Write the wtmp shutdown entry without shutting down the system:

`poweroff --wtmp-only`
