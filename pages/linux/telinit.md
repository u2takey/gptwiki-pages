# telinit 
## chatgpt 
The "telinit" command is a command used to change the runlevel of a Unix or Linux system.

Runlevels are levels of system operation, each with a different set of processes and services running. Changing the runlevel with telinit can be useful in performing system maintenance or troubleshooting.

The basic syntax of the telinit command is:

telinit [runlevel]

The "runlevel" argument can be a single digit from 0 to 6, which represents the different runlevels of the system:

0 – Halt the system
1 – Single-user mode
2 – Multi-user mode without Networking
3 – Multi-user mode with Networking
4 – Undefined
5 – GUI mode
6 – Reboot the system

For example, to switch to runlevel 3 (multi-user mode with networking), you would use the following command:

telinit 3

Alternatively, you can use the "init" command with the runlevel argument to achieve the same result:

init 3

Note that changing the runlevel requires root (administrative) privileges, so you may need to prefix the command with "sudo" and enter your password. 

## tldr 
 
> Change SysV runlevel.
> Since the concept SysV runlevels is obsolete the runlevel requests will be transparently translated into systemd unit activation requests.
> More information: <https://manned.org/telinit>.

- Power off the machine:

`telinit 0`

- Reboot the machine:

`telinit 6`

- Change SysV run level:

`telinit {{2|3|4|5}}`

- Change to rescue mode:

`telinit 1`

- Reload daemon configuration:

`telinit q`

- Do not send a wall message before reboot/power-off (6/0):

`telinit --no-wall {{value}}`
