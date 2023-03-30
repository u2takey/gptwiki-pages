# vgdisplay 
## chatgpt 
The "vgdisplay" command is a command-line utility tool used in Linux systems. It is part of the LVM (Logical Volume Manager) package and is used to display the attributes of the physical and logical volumes in a volume group.

When executed, the "vgdisplay" command displays various information about the volume group, such as the name of the volume group, the number of physical volumes allocated to the group, the size of the total physical volumes, the number of logical volumes, and the number of physical extents allocated to the volume group.

The output of the "vgdisplay" command also includes details about the physical volumes that make up the volume group, such as the physical volume's name, its size, and the free space available on each physical volume.

The "vgdisplay" command is used by system administrators to get an overview of the storage resources available on the system, which can help them manage storage volumes and allocate resources more efficiently. Additionally, it can be used to diagnose issues related to the storage media or the logical volumes. 

## tldr 
 
> Display information about Logical Volume Manager (LVM) volume groups.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/vgdisplay.8.html>.

- Display information about all volume groups:

`sudo vgdisplay`

- Display information about volume group vg1:

`sudo vgdisplay {{vg1}}`
