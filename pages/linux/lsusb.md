# lsusb 
## chatgpt 
The "lsusb" command is a Linux command that is used to list all USB devices that are currently connected to the computer. When it is executed, it will display a list of USB devices along with their vendor and product IDs. 

Here's a breakdown of the command:

- "ls" stands for "list" and is a common command used in Linux to list information about files and directories.
- "usb" stands for "Universal Serial Bus", which is the standard interface used to connect devices to a computer. 
- So when "lsusb" is typed into the terminal and executed, it tells the computer to list all USB devices currently attached to it.

This command can be useful when troubleshooting USB devices that are not working properly, checking if a device is properly detected by the system, and identifying the make and model of a particular USB device. 

## tldr 
 
> Display information about USB buses and devices connected to them.
> More information: <https://manned.org/lsusb>.

- List all the USB devices available:

`lsusb`

- List the USB hierarchy as a tree:

`lsusb -t`

- List verbose information about USB devices:

`lsusb --verbose`

- List detailed information about a USB device:

`lsusb -D {{device}}`

- List devices with a specified vendor and product ID only:

`lsusb -d {{vendor}}:{{product}}`
