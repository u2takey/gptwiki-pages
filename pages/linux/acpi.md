# acpi 
## chatgpt 
The acpi command is used to display information about the Advanced Configuration and Power Interface (ACPI) of a Linux system. ACPI is an open standard that defines power management and configuration interfaces between hardware, firmware (BIOS, UEFI), and operating system.

When the acpi command is executed, it can show the following information:

- Battery: the status, remaining capacity, and charging status of the battery
- Thermal: temperature readings of the CPU and other hardware components
- Fan: fan speed and rotation status
- Power: power source and energy usage information
- Processor: CPU details such as the current frequency, temperature, and power usage
- Sleep states: the sleep states supported by the system and the current state

To execute the acpi command and view the ACPI information, open a terminal window and type:

```
acpi
```

You can also add options after the command to specify which information you want to display. For example:

```
acpi -b     # show battery information
acpi -t     # show thermal information
acpi -f     # show fan information
acpi -V     # show battery and adapter information
```

Overall, the acpi command is a useful tool for monitoring power management and system health of a Linux system. 

## tldr 
 
> Shows battery status or thermal information.
> More information: <https://sourceforge.net/projects/acpiclient/files/acpiclient/>.

- Show battery information:

`acpi`

- Show thermal information:

`acpi -t`

- Show cooling device information:

`acpi -c`

- Show thermal information in Fahrenheit:

`acpi -tf`

- Show all information:

`acpi -V`

- Extract information from `/proc` instead of `/sys`:

`acpi -p`
