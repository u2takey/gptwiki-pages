# cfdisk 
## chatgpt 
CFDisk is a command line partitioning tool on Linux systems, which allows users to create, delete or modify partitions on their hard drives. It is an interactive tool that displays a graphical user interface for managing partitions.

When you run the command "cfdisk" in the terminal, you'll be presented with a screen that shows your available hard drives and their partitions. You can then select which drive you want to modify, and create new partitions or delete existing ones.

Here are some of the main features of CFDisk:

- Supports MBR and GPT partition schemes.
- Displays information about the partition table and shows free space on the disk.
- Allows you to create primary, extended, and logical partitions with different filesystems such as ext4, NTFS, FAT32 etc.
- Includes options to set partition size, create bootable partitions and toggle partition boot flags.
- Supports navigation using arrow keys and provides a help menu accessible with the F1 key.
- Requires sudo permissions to run as it requires root access to modify your disk.

Overall, the cfdisk command is a useful tool for Linux users who need to manage partitions on their hard drives. 

## tldr 
 
> A program for managing partition tables and partitions on a hard disk using a curses UI.
> More information: <https://manned.org/cfdisk>.

- Start the partition manipulator with a specific device:

`cfdisk {{/dev/sdX}}`

- Create a new partition table for a specific device and manage it:

`cfdisk --zero {{/dev/sdX}}`
