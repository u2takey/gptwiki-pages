# wdctl 
## chatgpt 
The "wdctl" command is used to manage watchdog timers on a system. A watchdog timer is a hardware device or software feature that is used to prevent a system from becoming unresponsive, by automatically resetting the system if it detects that the software has stopped functioning. 

The "wdctl" command is mainly used to start, stop or check the status of a watchdog timer on a system. The specific parameters of the command may differ depending on the operating system and the type of watchdog timer being used.

Here are some common parameters used with the "wdctl" command:

- "-t" or "--timeout": This parameter is used to set the timeout value of the watchdog timer. The timeout value is the amount of time that the system has to respond before the watchdog timer triggers a system reset. This could be specified in seconds, minutes, or hours depending on the timer.
- "-s" or "--status": This parameter is used to check the current status of the watchdog timer. It will display the timeout value, as well as the time remaining before the next system reset.
- "-a" or "--activate": This parameter is used to activate the watchdog timer. Once activated, the timer will start monitoring the system for any signs of unresponsiveness.
- "-d" or "--deactivate": This parameter is used to deactivate the watchdog timer. Once deactivated, the timer will stop monitoring the system.

Overall, the "wdctl" command is an important tool for system administrators who need to ensure that their systems are always running smoothly and that any potential problems are caught and addressed quickly. 

## tldr 
 
> Show the hardware watchdog status.
> More information: <https://manned.org/wdctl>.

- Display the watchdog status:

`wdctl`

- Display the watchdog status in a single line in key-value pairs:

`wdctl --oneline`

- Display only specific watchdog flags (list is driver specific):

`wdctl --flags {{flag_list}}`
