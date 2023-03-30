# shutdown 
## chatgpt 
The "shutdown" command is used to shut down or reboot a computer. It allows the user to initiate a system shutdown or restart from the command line interface without having to go through the graphical user interface.

Syntax:
shutdown [OPTIONS...] [TIME] [MESSAGE]

Options:
- -h or --halt: This option shuts down the system and turns off power (also referred to as a "halt" or "power off").
- -r or --reboot: This option shuts down the system and then restarts it.
- -c or --cancel: This option cancels a previously scheduled shutdown or reboot.
- -t or --time: This option specifies the time when the shutdown or reboot will occur, which can be immediately or at a specific time (in minutes or hours).
- -k or --kmsg: This option writes a message to the kernel log to announce the shutdown or reboot.
- -n or --no-wall: This option prevents a wall message from being sent to all users before the shutdown or reboot occurs.
- -f or --force: This option forces all processes to terminate without warning.

Message:
The message argument specifies a custom message to be displayed to all users before the shutdown or reboot occurs.

Example:
To shut down the system immediately with a custom message, you can use the following command:
shutdown -h now "System is going down for maintenance"

This will halt the operating system and power off the computer, displaying the specified system message to all users. 

## tldr 
 
> Shutdown and reboot the system.
> More information: <https://manned.org/shutdown.8>.

- Power off (halt) immediately:

`shutdown -h now`

- Reboot immediately:

`shutdown -r now`

- Reboot in 5 minutes:

`shutdown -r +{{5}} &`

- Shutdown at 1:00 pm (Uses 24h clock):

`shutdown -h 13:00`

- Cancel a pending shutdown/reboot operation:

`shutdown -c`
