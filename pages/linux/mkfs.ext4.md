# mkfs.ext4 
## chatgpt 
The `mkfs.ext4` command is a Linux command used to create an Ext4 filesystem on a partition or a device. This command is used to initialize a new file system on a disk partition or a disk device, making it ready for data storage.

Here is a breakdown of the command parameters:

- `mkfs` - this command stands for make filesystem, and it is used to create a new filesystem on a partition or a device.
- `ext4` - this is the type of filesystem that will be created, in this case, it is the Ext4 filesystem.
- Parameters - the command can include other parameters such as '-t' to specify the filesystem type and '-c' to perform a surface scan before creating the filesystem.

To use this command, you need to have administrative privileges in Linux since it requires writing data to block devices that are owned by the root user. Before running the command, ensure that you have backed up your data since running the command will erase all data on the target partition or device. 

Overall, the `mkfs.ext4` command is a powerful tool that can be used to create a new Ext4 filesystem that can be used for data storage. 

## tldr 
 
> Creates an ext4 filesystem inside a partition.
> More information: <https://manned.org/mkfs.ext4>.

- Create an ext4 filesystem inside partition 1 on device b (`sdb1`):

`sudo mkfs.ext4 {{/dev/sdb1}}`

- Create an ext4 filesystem with a volume-label:

`sudo mkfs.ext4 -L {{volume_label}} {{/dev/sdb1}}`
