# addpart 
## chatgpt 
The "addpart" command is used in Linux operating systems to create a new partition on a specified storage device. This command is typically used for hard disk drives, solid-state drives, USB drives, or any other type of storage device that can be accessed by the operating system.

The syntax of the "addpart" command is as follows: 

addpart [options] <device> <start> <end> 

- "options" refer to any additional flags or arguments that can be passed to the command. 

- "device" specifies the storage device on which the new partition is to be created, such as /dev/sda, /dev/sdb, etc. 

- "start" specifies the start sector or block number which the new partition should occupy. 

- "end" specifies the end sector or block number which the new partition should occupy.

Some commonly used options with the addpart command are:

- -r, --readonly: creates a read-only partition
- -u, --uuid <uuid>: sets the UUID of the new partition
- -t, --type <type>: sets the partition type (e.g. ext4, ntfs, fat32)

Note that the addpart command is typically used by advanced users or system administrators, as it involves dealing with partitioning and formatting of storage devices. It is important to use this command with caution, as creating or modifying partitions can potentially result in data loss on the device if not done properly. It is always recommended to back up important data before making any changes to the disk partitions. 

## tldr 
 
> Tells the Linux kernel about the existence of the specified partition.
> The command is a simple wrapper around the `add partition` ioctl.
> More information: <https://manned.org/addpart>.

- Tell the kernel about the existence of the specified partition:

`addpart {{device}} {{partition}} {{start}} {{length}}`
