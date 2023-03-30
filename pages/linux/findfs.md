# findfs 
## chatgpt 
The "findfs" command is used to find the file system that corresponds to a particular device or label. It is commonly used in Linux systems to determine the partition, file system, or file label that a particular file belongs to.

The basic syntax of the "findfs" command is as follows:

    findfs [OPTION]... [DEVICE|LABEL|UUID]

Here, "DEVICE" can be the name or path of a block device, "LABEL" can be the label of a file system, and "UUID" can be the universally unique identifier of a file system.

Some of the commonly used options with the "findfs" command are:

- "-t TYPE": Specifies the file system type to be searched for.
- "-s": Prints the UUID and other details of the file system in addition to the file system path.
- "-l": Lists all the known file systems and their corresponding devices.

For example, the following command will find the file system that corresponds to the device "/dev/sda1" and display its UUID:

    findfs -s /dev/sda1

This command will list all known file systems and their corresponding devices:

    findfs -l

Overall, the "findfs" command is a useful tool for locating file systems associated with devices or labels in Linux systems. 

## tldr 
 
> Finds a filesystem by label or UUID.
> More information: <https://mirrors.edge.kernel.org/pub/linux/utils/util-linux>.

- Search block devices by filesystem label:

`findfs LABEL={{label}}`

- Search by filesystem UUID:

`findfs UUID={{uuid}}`

- Search by partition label (GPT or MAC partition table):

`findfs PARTLABEL={{partition_label}}`

- Search by partition UUID (GPT partition table only):

`findfs PARTUUID={{partition_uuid}}`
