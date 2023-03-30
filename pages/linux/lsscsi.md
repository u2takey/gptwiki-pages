# lsscsi 
## chatgpt 
The lsscsi command is used to list all SCSI/SATA devices on your system. It stands for List SCSI devices. It provides a concise summary of SCSI devices installed on the system like the type of device, its vendor, and model name, and a few other details.

When executed, it scans the SCSI subsystem and generates a list of SCSI/SATA devices connected to the system, including disks, CD/DVD drives, and tape drives, in a human-readable format.

The following information is usually displayed for each device:

- Device name: This is the name of the SCSI device on the system.
- Type: This is the type of device, such as a CD-ROM, Disk, or DVD.
- Vendor: This is the name of the manufacturer of the device.
- Model: This is the model name or number of the device and its revision.
- Rev: This is the revision number of the device firmware.
- HCTL: This is the host controller, target, and logical unit information for the device.
- Size/GB: This is the size of the device in gigabytes.

Overall, the lsscsi command is useful for troubleshooting purposes, especially when you need to identify SCSI/SATA devices connected to your system. 

## tldr 
 
> List SCSI devices (or hosts) and their attributes.
> More information: <https://manned.org/lspci>.

- List all SCSI devices:

`lsscsi`

- List all SCSI devices with detailed attributes:

`lsscsi -L`

- List all SCSI devices with human-readable disk capacity:

`lsscsi -s`
