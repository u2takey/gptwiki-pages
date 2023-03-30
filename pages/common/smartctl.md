# smartctl 
## chatgpt 
Smartctl stands for SMART Control, and it is a command-line tool used to monitor the health and performance of storage devices such as hard disk drives (HDD), solid-state drives (SSD), and NVMe drives. It is available on most Unix-based operating systems like Linux, FreeBSD, OpenBSD, and macOS.

The command syntax for smartctl is as follows:

```
smartctl [options] device
```

Here is a brief explanation of the main options and their purposes:

- `-a`: Displays all available SMART information for the device.
- `-H`: Shows the overall health status of the device.
- `-c`: Displays the device's SMART capabilities.
- `-t <test>`: Starts a specific SMART self-test for the device.
- `-l <num>`: Shows the device's SMART log directory (numbered).

The options above are just a few examples of what smartctl can do - there are many other commands and modifiers available. When using smartctl, the device argument refers to the storage device being monitored. It can be specified as a device node name such as "/dev/sda" or "/dev/nvme0n1", or as an ATAPI device name such as "/dev/cdrom". 

Overall, smartctl is invaluable for checking the health of your storage devices and predicting possible issues early on. It allows you to monitor essential parameters like temperature, power-on hours, bad sectors count, and reallocate sector count, among others. Its flexibility and extensive output make it a go-to tool for technicians, system administrators, and everyday users alike. 

## tldr 
 
> Monitor disk health including SMART data.
> More information: <https://www.smartmontools.org>.

- Display SMART health summary:

`sudo smartctl --health {{/dev/sdX}}`

- Display device information:

`sudo smartctl --info {{/dev/sdX}}`

- Start a short self-test in the background:

`sudo smartctl --test short {{/dev/sdX}}`

- Display current/last self-test status and other SMART capabilities:

`sudo smartctl --capabilities {{/dev/sdX}}`

- Display exhaustive SMART data:

`sudo smartctl --all {{/dev/sdX}}`
