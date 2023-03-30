# partprobe 
## chatgpt 
partprobe is a command in Linux that is used to inform the operating system kernel about changes in partitions on a hard disk. It allows the system to detect any changes made to partitions, whether they are added or removed, without the need to restart the computer.

When a partition is created or deleted on a hard disk, the kernel may not be aware of these changes until the system is restarted. This can lead to problems if the system needs to access the newly created partitions immediately. The partprobe command prevents this issue as it scans the hard disk partition table and informs the kernel of any changes made to the partitions.

The syntax of the partprobe command is simple. We can simply use the command with the name of the device whose partition table we want to update:

partprobe [device-name]

For example, to update the partition table of the /dev/sda device, we can use the following command:

partprobe /dev/sda

This command scans the partition table of the /dev/sda device and updates the kernel with any changes made to partitions. Once executed, the kernel will recognize any new partitions or changes in existing partitions, and the system will be able to access them without restarting.

In summary, the partprobe command is a convenient tool for updating the kernel about changes in partitions, making it unnecessary to restart the system or unmount the partitions manually. 

## tldr 
 
> Notify the operating system kernel of partition table changes.
> More information: <https://manned.org/partprobe>.

- Notify the operating system kernel of partition table changes:

`sudo partprobe`

- Notify the kernel of partition table changes and show a summary of devices and their partitions:

`sudo partprobe --summary`

- Show a summary of devices and their partitions but don't notify the kernel:

`sudo partprobe --summary --dry-run`
