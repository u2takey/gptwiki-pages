# dumpe2fs 
## chatgpt 
The "dumpe2fs" command is a Linux utility that is used to display detailed information about the ext2, ext3, and ext4 file systems. It is a command-line tool that displays information such as the file system version, size, block size, reserved block count, inode count, number of free blocks, and various other details about the file system.

The "dumpe2fs" command requires the name of the block device that contains the ext2, ext3, or ext4 file system as an argument. It then displays the detailed information about the file system in a human-readable format.

Some of the common options used with this command are:

- "-h" or "--help": Displays a brief help message about how to use the command.
- "-i" or "--inode": Displays information about a specific inode (an index node of a file or directory).
- "-x" or "--extended": Displays extended information about the file system, including the location of the superblock, block group information, and feature flags.

Overall, the "dumpe2fs" command is a powerful tool for displaying detailed information about file systems on Linux systems. It can be useful for troubleshooting file system issues and for gaining a better understanding of how the file system works. 

## tldr 
 
> Print the super block and blocks group information for ext2/ext3/ext4 filesystems.
> Unmount the partition before running this command using `umount {{device}}`.
> More information: <https://manned.org/dumpe2fs>.

- Display ext2, ext3 and ext4 filesystem information:

`dumpe2fs {{/dev/sdXN}}`

- Display the blocks which are reserved as bad in the filesystem:

`dumpe2fs -b {{/dev/sdXN}}`

- Force display filesystem information even with unrecognizable feature flags:

`dumpe2fs -f {{/dev/sdXN}}`

- Only display the superblock information and not any of the block group descriptor detail information:

`dumpe2fs -h {{/dev/sdXN}}`

- Print the detailed group information block numbers in hexadecimal format:

`dumpe2fs -x {{/dev/sdXN}}`
