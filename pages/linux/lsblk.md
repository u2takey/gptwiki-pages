# lsblk 
## chatgpt 
The "lsblk" command is a Linux command that is used to list information about all available block devices on your system. The command provides a detailed list of all storage devices such as hard disks, USB drives, and CD-ROMs, and their corresponding partitions.

When you execute the "lsblk" command, it displays a table-like output showing the device names, the partitions, the size of the block devices, and how they are connected to the system. The output is organized into columns, and the column headers usually include device name (NAME), mount point (MOUNTPOINT), and file system type (FSTYPE).

The "lsblk" command is often used by system administrators to identify available storage devices and to determine their properties, including their size and capacity. This information can be useful in a variety of situations, such as when configuring partitioning and file systems, managing backups, or troubleshooting storage-related issues. 

## tldr 
 
> Lists information about devices.
> More information: <https://manned.org/lsblk>.

- List all storage devices in a tree-like format:

`lsblk`

- Also list empty devices:

`lsblk -a`

- Print the SIZE column in bytes rather than in a human-readable format:

`lsblk -b`

- Output info about filesystems:

`lsblk -f`

- Use ASCII characters for tree formatting:

`lsblk -i`

- Output info about block-device topology:

`lsblk -t`

- Exclude the devices specified by the comma-separated list of major device numbers:

`lsblk -e {{1,7}}`

- Display a customized summary using a comma-separated list of columns:

`lsblk --output {{NAME}},{{SERIAL}},{{MODEL}},{{TRAN}},{{TYPE}},{{SIZE}},{{FSTYPE}},{{MOUNTPOINT}}`
