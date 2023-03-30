# partx 
## chatgpt 
The Partx command is a utility program used in Unix systems to control and view partition tables. This command is used to create, remove, and manipulate partition tables on a block device.

The command has various options and arguments that can be used to control the partition table. One common use of Partx is to update the kernel's partition table after resizing a partition, adding a new partition, or removing an existing one.

Here's an overview of some of the commonly used options and arguments with Partx command:

- -a, --add : Adds a new partition to the partition table.
- -d, --delete : Deletes a partition from the partition table.
- -g, --show-guid : Shows the partition table's GPT GUID.
- -u, --update : Updates the kernel's partition data.
- -r, --raw : Uses the raw sector numbers instead of the partition number to specify a partition.

Overall, Partx is a powerful command that can be used to modify and manage partition tables on block devices. 

## tldr 
 
> Parse a partition table and tell the kernel about it.
> More information: <https://man7.org/linux/man-pages/man8/partx.8.html>.

- List the partitions on a block device or disk image:

`sudo partx --list {{path/to/device_or_disk_image}}`

- Add all the partitions found in a given block device to the kernel:

`sudo partx --add --verbose {{path/to/device_or_disk_image}}`

- Delete all the partitions found from the kernel (does not alter partitions on disk):

`sudo partx --delete {{path/to/device_or_disk_image}}`
