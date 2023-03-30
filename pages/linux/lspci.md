# lspci 
## chatgpt 
lspci stands for "List Peripheral Component Interconnect", and it is a command-line utility used in Linux and other Unix-like operating systems to display information about all connected PCI (Peripheral Component Interconnect) devices. When this command is executed, it scans your computer's PCI bus and identifies all the devices connected to it, such as graphics cards, sound cards, network cards, and other hardware components.

The output of the lspci command includes information about the devices, such as their vendor ID, device ID, subsystem ID, class, and driver information. The information provided can be useful for troubleshooting hardware issues, identifying devices that may not be working correctly, and finding driver information for the devices.

The lspci command can be further customized using different options to display specific information or filter the output based on specific criteria. For example, you can use the -v option to display verbose information about each device, or the -d option to filter the output based on specific vendor or device IDs.

Overall, the lspci command is a powerful tool for viewing information about the hardware components connected to your computer and can be very useful in diagnosing and troubleshooting issues related to hardware. 

## tldr 
 
> List all PCI devices.
> More information: <https://manned.org/lspci>.

- Show a brief list of devices:

`lspci`

- Display additional info:

`lspci -v`

- Display drivers and modules handling each device:

`lspci -k`

- Show a specific device:

`lspci -s {{00:18.3}}`

- Dump info in a readable form:

`lspci -vm`
