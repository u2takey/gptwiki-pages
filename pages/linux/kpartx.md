# kpartx 
## chatgpt 
kpartx is a Linux command that is used to create device mappings for the partitions in a disk image or a physical disk. It is a Linux specific utility that allows you to mount partitions in a disk image or physical disk as individual devices.

When you run the kpartx command, it scans the disk image or physical disk and creates device mappings for each partition. It creates device files in the /dev/mapper directory for each partition so that you can access them.

The command has various options that can be used to adjust its behavior. Some of the common options are:

- -a : Add partition mappings for all partitions in the disk image or physical disk.
- -d : Delete partition mappings.
- -u : Update the device mappings.
- -f : Force the creation of device mappings even if they already exist.

Overall, the kpartx command is very useful for working with disk images or physical disks with multiple partitions, as it simplifies the process of accessing individual partitions as separate devices. 

## tldr 
 
> Create device maps from partition tables.
> More information: <https://manned.org/kpartx>.

- Add partition mappings:

`kpartx -a {{whole_disk.img}}`

- Delete partition mappings:

`kpartx -d {{whole_disk.img}}`

- List partition mappings:

`kpartx -l {{whole_disk.img}}`
