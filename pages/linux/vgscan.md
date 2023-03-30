# vgscan 
## chatgpt 
The "vgscan" command is used in Linux to scan all the available physical volumes (hard disks, disk partitions, RAID arrays, etc.) on the system and detect any new or changed Volume Groups (VGs) and Logical Volumes (LVs). 

The command uses the information from the metadata stored on the physical volumes which describes the organization of the VGs and LVs. This information is used to rebuild the logical volume database in the system's cache memory.

This command can be used to update the system's list of available VGs and LVs after making changes to disk partitions, adding new drives or RAID arrays, or after a system crash which resulted in the corruption of the logical volume database. Once the system has scanned and detected the VGs and LVs, they can be activated for use by the operating system. 

In summary, the "vgscan" command is used to detect and maintain the logical volumes and volume groups on a Linux system. It is an essential part of managing storage on a Linux system. 

## tldr 
 
> Scan for volume groups on all supported Logical Volume Manager (LVM) block devices.
> See also `lvm`, `vgchange`.
> More information: <https://manned.org/vgscan>.

- Scan for volume groups and print information about each group found:

`sudo vgscan`

- Scan for volume groups and add the special files in `/dev`, if they don't already exist, needed to access the logical volumes in the found groups:

`sudo vgscan --mknodes`
