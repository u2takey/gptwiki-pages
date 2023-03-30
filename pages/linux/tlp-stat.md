# tlp-stat 
## chatgpt 
The "tlp-stat" command is used to display the current configuration and status of TLP (or TLPUI) on a Linux system. TLP is a power management utility, which is used to optimize the power consumption of a laptop (or desktop) running on battery power by adjusting various hardware settings (such as CPU frequency scaling, screen brightness, etc.). 

When you run the "tlp-stat" command, it will display the following information:

1. TLP version number

2. TLP configuration parameters - this includes information about various power management settings and their current values, such as CPU scaling, WiFi power saving mode, Bluetooth power management, etc.

3. ACPI information - this displays information about the ACPI (Advanced Configuration and Power Interface) devices on the system, such as thermal sensors, battery status, etc.

4. Kernel modules - this lists the kernel modules loaded on the system and their status.

5. Debug messages - this displays any relevant debug messages, which can be helpful in identifying any issues or problems with TLP or the system's power management settings.

Overall, the "tlp-stat" command is a useful tool for troubleshooting power management issues and optimizing power consumption on Linux systems. 

## tldr 
 
> A tool to generate TLP status reports.
> See also `tlp`.
> More information: <https://linrunner.de/tlp/usage/tlp-stat>.

- Generate status report with configuration and all active settings:

`sudo tlp-stat`

- Show battery information:

`sudo tlp-stat -b`

- Show configuration:

`sudo tlp-stat -c`
