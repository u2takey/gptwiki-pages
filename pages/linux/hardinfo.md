# hardinfo 
## chatgpt 
The "hardinfo" command in Linux is used to display detailed information about the hardware components of the system. It is a graphical tool that provides information about the CPU, RAM, storage devices, motherboard, network interfaces, graphics card, and other hardware components.

When you run the "hardinfo" command in the terminal, it opens the hardinfo graphical interface, displaying the hardware components arranged in different categories. You can click on any category to expand it and view the detailed information about the components.

The "System Summary" category provides an overview of the hardware components, BIOS version, and system resources like memory and swap usage.

The "Devices" category displays information about the connected hardware devices, such as USB devices, printers, and scanners.

The "Network" category provides information about the network interfaces and their configurations.

The "Sensors" category displays sensor data such as CPU temperature, fan speed, and voltage.

The "Benchmark" category provides performance benchmarks for the CPU, RAM, and disk drives.

Overall, the hardinfo command is a useful tool for system administrators, technicians, and normal users to collect hardware information and diagnose hardware-related issues. 

## tldr 
 
> Show hardware information in GUI window.
> More information: <https://github.com/lpereira/hardinfo>.

- Start hardinfo:

`hardinfo`

- Print report to standard output:

`hardinfo -r`

- Save report to HTML file:

`hardinfo -r -f html > hardinfo.html`
