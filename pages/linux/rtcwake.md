# rtcwake 
## chatgpt 
The `rtcwake` command is a utility in Linux and UNIX environments that schedules the system to automatically enter a low-power state or wake up at a specific time. It is typically used to save power on devices such as laptops or servers.

Here are the various options and their meanings for the `rtcwake` command:

- `-m`: Specifies the suspend mode to use. This can be one of `mem` (suspend to RAM), `disk` (suspend to disk), or `off` (power off the system). By default, `mem` is used.
- `-s`: Specifies the number of seconds until the system wakes up. This can be used instead of the absolute wake-up time.
- `-t`: Specifies the absolute wake-up time, in the format `YYYY-MM-DD HH:MM:SS`.
- `-u`: Specifies the wake-up time in UTC instead of the local time zone.
- `-l`: Specifies the option to use local time instead of UTC.
- `-d`: Activates the low-level driver mode if possible. This is typically used for debugging and testing purposes.
- `-h`, `-V`: Displays help or version information respectively.

Here is an example of how you can use the `rtcwake` command:

```
sudo rtcwake -m mem -s 300
```

This command will put the system into a suspend state (`mem`) for the next five minutes (`-s 300`). After that period of time, the system will wake back up.

Overall, the `rtcwake` command is a useful tool for managing power consumption on Linux devices while also helping you schedule tasks or events to occur at specific times. 

## tldr 
 
> Enter a system sleep state until specified wakeup time relative to your BIOS clock.
> More information: <https://manned.org/rtcwake>.

- Show whether an alarm is set or not:

`sudo rtcwake -m show -v`

- Suspend to RAM and wakeup after 10 seconds:

`sudo rtcwake -m mem -s {{10}}`

- Suspend to disk (higher power saving) and wakeup 15 minutes later:

`sudo rtcwake -m disk --date +{{15}}min`

- Freeze the system (more efficient than suspend-to-RAM but version 3.9 or newer of the Linux kernel is required) and wakeup at a given date and time:

`sudo rtcwake -m freeze --date {{YYYYMMDDhhmm}}`

- Disable a previously set alarm:

`sudo rtcwake -m disable`

- Perform a dry run to wakeup the computer at a given time. (Press Ctrl + C to abort):

`sudo rtcwake -m on --date {{hh:ss}}`
