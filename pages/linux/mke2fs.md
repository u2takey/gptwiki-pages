# mke2fs 
## chatgpt 
mke2fs stands for make ext2/ext3/ext4 filesystem. It is a command used to create a new ext2, ext3, or ext4 file system on a disk partition or a block device.

The syntax for the mke2fs command is:

mke2fs [options] device [block count]

Some of the commonly used options are:

- -t ext2/ext3/ext4: Specifies the type of file system to be created.
- -c: Checks for bad blocks on the device.
- -L label: Assigns a label to the file system.
- -m percentage: Reserves a percentage of the file system for use by the superuser.
- -j: Creates an ext3 file system with a journal.
- -O feature: Enables optional features in the file system, such as compression and encryption.

The device parameter specifies the device or partition on which the file system will be created. The block count parameter is optional and specifies the number of blocks to be used for the file system. If it is not specified, mke2fs will use the maximum number of blocks available on the device.

Once executed, the mke2fs command formats the specified device or partition with the specified file system type and creates the necessary directory structures and metadata for the file system. The new file system can then be mounted and used like any other file system. 

## tldr 
 
> Creates a Linux filesystem inside a partition.
> More information: <https://manned.org/mke2fs>.

- Create an ext2 filesystem in partition 1 of device b (`sdb1`):

`mkfs.ext2 {{/dev/sdb1}}`

- Create an ext3 filesystem in partition 1 of device b (`sdb1`):

`mkfs.ext3 {{/dev/sdb1}}`

- Create an ext4 filesystem in partition 1 of device b (`sdb1`):

`mkfs.ext4 {{/dev/sdb1}}`
