# upower 
## chatgpt 
`upower` is a Linux command-line utility for querying and interacting with the power management subsystem of the system.

This command can be used to get information about the power supply, batteries and power consumption on a Linux system. It can display the battery status, battery percentage, power source, the time remaining for a battery to be fully charged or fully discharged, and other information related to the power management.

Here are some examples of how to use the `upower` command:

- Get all devices:
```
upower -e
```
- Get information about the battery:
```
upower -i /org/freedesktop/UPower/devices/battery_BAT0
```
- List power supply details:
```
upower -d
```
- Get the percentage of battery left:
```
upower -i /org/freedesktop/UPower/devices/battery_BAT0 | grep percentage
```
- Get the time remaining to fully charge the battery:
```
upower -i /org/freedesktop/UPower/devices/battery_BAT0 | grep "time to full"
```

Overall, `upower` is a useful tool to monitor battery and power consumption on a Linux system. 

## tldr 
 
> System utility to provide power and battery information and statistics.
> More information: <https://upower.freedesktop.org/docs/upower.1.html>.

- Display power and battery information:

`upower --dump`

- List all power devices:

`upower --enumerate`

- Watch for and print power status changes:

`upower --monitor`

- Watch for and print detailed power status changes:

`upower --monitor-detail`

- Display version:

`upower --version`
