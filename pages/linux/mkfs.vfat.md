# mkfs.vfat 
## chatgpt 
The `mkfs.vfat` command is used to create a file system on a storage device (such as a disk or a USB drive) using the FAT (File Allocation Table) file system format. Here is a detailed breakdown of the different parts of the command:

- `mkfs`: This stands for "make file system" and is a command used to create a new file system on a storage device.
- `.vfat`: This is an option that specifies the file system format to be used. In this case, `vfat` refers to the FAT file system format.
 
The command typically requires an additional parameter specifying the storage device that you want to format with a FAT file system.

For example, `mkfs.vfat /dev/sdb1` would create a new FAT file system on the storage device located at `/dev/sdb1`. 

## tldr 
 
> Creates an MS-DOS filesystem inside a partition.
> More information: <https://manned.org/mkfs.vfat>.

- Create a vfat filesystem inside partition 1 on device b (`sdb1`):

`mkfs.vfat {{/dev/sdb1}}`

- Create filesystem with a volume-name:

`mkfs.vfat -n {{volume_name}} {{/dev/sdb1}}`

- Create filesystem with a volume-id:

`mkfs.vfat -i {{volume_id}} {{/dev/sdb1}}`

- Use 5 instead of 2 file allocation tables:

`mkfs.vfat -f 5 {{/dev/sdb1}}`
