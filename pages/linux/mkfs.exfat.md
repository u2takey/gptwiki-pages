# mkfs.exfat 
## chatgpt 
The mkfs.exfat command is a Linux command used to create a file system of the ExFAT type. ExFAT is an extended file allocation table that is used in flash drives, memory cards, and other external storage devices, allowing them to be used between multiple operating systems and devices.

The command syntax for mkfs.exfat is as follows:

mkfs.exfat [options] [device]

Where, 

- options: specifies the various optional parameters to customize the file system creation. There are many options available like -n for specifying the volume label, -s for specifying the sector size of file system etc.
- device: specifies the device or partition where the ExFAT file system is to be created.

Once the command is executed, it will format the device with ExFAT file system, which will erase all data from the device. After formatting, the device can be mounted and accessed to store data in it. 

In summary, the mkfs.exfat command is used to create an ExFAT file system on a specified device, with options available to customize the file system settings. 

## tldr 
 
> Creates an exfat filesystem inside a partition.
> More information: <https://manned.org/mkfs.exfat>.

- Create an exfat filesystem inside partition 1 on device b (`sdb1`):

`mkfs.exfat {{/dev/sdb1}}`

- Create filesystem with a volume-name:

`mkfs.exfat -n {{volume_name}} {{/dev/sdb1}}`

- Create filesystem with a volume-id:

`mkfs.exfat -i {{volume_id}} {{/dev/sdb1}}`
