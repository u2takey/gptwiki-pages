# fdisk 
## chatgpt 
fdisk is a command-line partitioning utility used to create, delete, resize, and modify partitions on a hard disk. Below is a brief description of some of the commonly used options and flags with the fdisk command:

1. `fdisk -l`: It lists the available partitions of all hard disks. 

2. `fdisk /dev/sdX`: It opens the hard disk partition of /dev/sdX, where X represents the drive letter.

3. `m`: This option shows the available fdisk commands.

4. `n`: This option is used to create a new partition.

5. `d`: This option is used to delete a partition.

6. `t`: This option is used to change the type of a partition.

7. `p`: This option is used to print the partition table of a hard disk.

8. `w`: This option is used to write the partition table changes to a hard disk.

Overall, the fdisk command is a powerful tool for managing partitions on a hard disk. It is important to exercise caution while using fdisk, as improper use can result in data loss or system instability. It is recommended to take a backup of important data before making any changes to partition tables. 

## tldr 
 
> A program for managing partition tables and partitions on a hard disk.
> See also: `partprobe`.
> More information: <https://manned.org/fdisk>.

- List partitions:

`sudo fdisk -l`

- Start the partition manipulator:

`sudo fdisk {{/dev/sdX}}`

- Once partitioning a disk, create a partition:

`n`

- Once partitioning a disk, select a partition to delete:

`d`

- Once partitioning a disk, view the partition table:

`p`

- Once partitioning a disk, write the changes made:

`w`

- Once partitioning a disk, discard the changes made:

`q`

- Once partitioning a disk, open a help menu:

`m`
