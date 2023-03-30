# parted 
## chatgpt 
Parted is a command-line tool used for partitioning hard disks or other storage devices. It is used to create, delete, resize, move and copy partitions, and it supports several filesystems including ext2, ext3, ext4, NTFS, FAT, and others.

The basic syntax of the parted command is as follows:

`parted [options] device [command [arguments]]`

Here, `device` refers to the storage device or hard drive you want to partition, and `command` is one of the partitioning commands or actions you want to perform.

Some of the commonly used options with the parted command are:

- `-l` or `--list`: List the partition tables on all available devices
- `-s` or `--script`: Run the command in non-interactive mode
- `-a` or `--align`: Set the alignment constraints for partitions
- `-m` or `--machine`: Display output in machine-readable format

Some of the commonly used commands with the parted command are:

- `mklabel` : Create a new partition table on the device
- `mkpart` : Create a new partition with specified type, file system, and size
- `resize` : Change the size of an existing partition
- `move` : Move a partition to a new location on the device
- `rm` : Remove a partition from the device

For example, to create a new primary partition of 50GB size on `/dev/sdb` device, we can use the following command:

`parted /dev/sdb mkpart primary 0GB 50GB`

Overall, the parted command is a powerful tool used for disk partition management and can be used to perform various operations on storage devices. 

## tldr 
 
> A partition manipulation program.
> See also: `partprobe`.
> More information: <https://www.gnu.org/software/parted/parted.html>.

- List partitions on all block devices:

`sudo parted --list`

- Start interactive mode with the specified disk selected:

`sudo parted {{/dev/sdX}}`

- Create a new partition table of the specified label-type:

`sudo parted --script {{/dev/sdX}} mklabel {{aix|amiga|bsd|dvh|gpt|loop|mac|msdos|pc98|sun}}`

- Show partition information in interactive mode:

`print`

- Select a disk in interactive mode:

`select {{/dev/sdX}}`

- Create a 16 GB partition with the specified filesystem in interactive mode:

`mkpart {{primary|logical|extended}} {{btrfs|ext2|ext3|ext4|fat16|fat32|hfs|hfs+|linux-swap|ntfs|reiserfs|udf|xfs}} {{0%}} {{16G}}`

- Resize a partition in interactive mode:

`resizepart {{/dev/sdXN}} {{end_position_of_partition}}`

- Remove a partition in interactive mode:

`rm {{/dev/sdXN}}`
