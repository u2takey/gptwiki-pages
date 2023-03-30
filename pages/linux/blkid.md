# blkid 
## chatgpt 
The "blkid" command is a Linux utility that is used to display information about available block devices, including their unique identifiers, file systems, labels, UUIDs, and other attributes. The blkid command can be used to query information about hard disks, partitions, USB drives, and various other storage devices connected to a system.

When running the "blkid" command, it scans the system for block devices and provides information about them in a formatted output. The output usually contains the device name, the file system type, and the unique identifier (UUID) of the device.

For example, a typical output of the "blkid" command for a hard disk might look like this:

/dev/sda1: UUID="4d41f2e4-8506-4f6d-b93d-1e3eaca5b7d5" TYPE="ext4"
/dev/sda2: UUID="7d5b1e3e-aca5-4f6d-b93d-4d41f2e48506" TYPE="swap"

In this example, the "blkid" command shows the UUID and the file system type of two partitions (/dev/sda1 and /dev/sda2) on the hard disk.

Overall, the "blkid" command is a useful tool for Linux system administrators to gather information about the various block devices connected to a system. 

## tldr 
 
> Lists all recognized partitions and their Universally Unique Identifier (UUID).
> More information: <https://manned.org/blkid>.

- List all partitions:

`sudo blkid`

- List all partitions in a table, including current mountpoints:

`sudo blkid -o list`
