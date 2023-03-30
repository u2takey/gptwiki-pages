# timedatectl 
## chatgpt 
The `timedatectl` command is used in Linux systems to control and view the system clock and time-related settings. It is used to view and modify the date, time, and timezone of the system.

When you run the `timedatectl` command, it will provide you with information about the current system time and date configuration. It displays information such as the current time and date, time zone, system clock accuracy, and whether or not the system clock is synchronized with an external time source.

We can also use the `timedatectl` command to modify the date, time, and timezone of the system. To modify the system time, use the `set-time` option with the new time in the HH:MM:SS format. Similarly, to change the system date or timezone, use the `set-date` or `set-timezone` options, respectively.

Overall, `timedatectl` is a useful command for managing time-related settings on Linux systems. It allows for easy configuration of system time, date, and timezone and provides accurate information about the current time configuration. 

## tldr 
 
> Control the system time and date.
> More information: <https://manned.org/timedatectl>.

- Check the current system clock time:

`timedatectl`

- Set the local time of the system clock directly:

`timedatectl set-time "{{yyyy-MM-dd hh:mm:ss}}"`

- List available timezones:

`timedatectl list-timezones`

- Set the system timezone:

`timedatectl set-timezone {{timezone}}`

- Enable Network Time Protocol (NTP) synchronization:

`timedatectl set-ntp on`

- Change the hardware clock time standard to localtime:

`timedatectl set-local-rtc 1`
