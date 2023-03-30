# dmidecode 
## chatgpt 
The "dmidecode" command is a Linux utility that provides detailed hardware information of the system, like motherboard, BIOS, system manufacturer, serial numbers, processor, and memory configuration. It reads data from the system's DMI (Desktop Management Interface) table, which is a database that holds system configuration details. 

When used in the terminal, the dmidecode command displays a wealth of information that is organized into several sections. For example, the system section of the output provides data on the computer's manufacturer, model name, BIOS version, product name, and other general details about the system. The processor section provides details about the installed CPU, such as its socket type, speed, and number of cores. The memory section gives information about the installed RAM, its speed, and the number of memory slots on the motherboard.  

Overall, the dmidecode command is a useful tool for system administrators and users who need to diagnose issues with their hardware or ensure that a system's hardware is compatible with a particular software or application. 

## tldr 
 
> Display the DMI (alternatively known as SMBIOS) table contents in a human-readable format.
> Requires root privileges.
> More information: <https://manned.org/dmidecode>.

- Show all DMI table contents:

`sudo dmidecode`

- Show the BIOS version:

`sudo dmidecode -s bios-version`

- Show the system's serial number:

`sudo dmidecode -s system-serial-number`

- Show BIOS information:

`sudo dmidecode -t bios`

- Show CPU information:

`sudo dmidecode -t processor`

- Show memory information:

`sudo dmidecode -t memory`
