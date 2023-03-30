# hwclock 
## chatgpt 
hwclock is a command used in Linux to access and adjust the hardware clock or real-time clock (RTC) of a system. The hardware clock is a separate clock that is powered by a small battery present on the motherboard, it provides a time reference for the system even when it is powered off.

The syntax of the hwclock command is:

```
hwclock [options]
```

Some of the most commonly used options with the hwclock command are:

- -s or --hctosys : This option is used to set the system time from the hardware clock.
- -w or --systohc : This option is used to set the hardware clock from the system time.
- -r or --show : This option is used to display the current hardware clock time.
- -c or --noadjfile : This option is used to disable the use of an adjtime file to synchronize the system clock with the hardware clock.

In addition to these options, there are other options available with the hwclock command that can be used according to the requirement. By default, the hwclock command operates in UTC time but it can be changed to local time by setting the UTC flag to no in the /etc/default/rcS file.

It is worth mentioning that hwclock command can only be used by the system administrator or root user in most cases because it involves accessing the hardware resources of the system. 

## tldr 
 
> Used for reading or changing the hardware clock. Usually requires root.
> More information: <https://manned.org/hwclock>.

- Display the current time as reported by the hardware clock:

`hwclock`

- Write the current software clock time to the hardware clock (sometimes used during system setup):

`hwclock --systohc`

- Write the current hardware clock time to the software clock:

`hwclock --hctosys`
