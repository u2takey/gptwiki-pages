# lvm 
## chatgpt 
The "lvm" command stands for "Logical Volume Manager" and is a utility that lets you manage storage devices in Linux. With LVM, you can create, resize, move, and delete partitions without having to shut down your Linux system or even unmount your filesystems.

Here are some commonly used options with LVM:

- pvcreate: This command is used to create a physical volume (a partition or a whole disk) that will be used by the LVM.
- vgcreate: This command creates a volume group (VG), which is a collection of physical volumes that are managed as a single unit.
- lvcreate: This command creates a logical volume (LV) within a volume group. The size and other attributes of the LV can be specified at the time of creation.
- lvextend: This command is used to extend a logical volume.
- lvreduce: This command is used to reduce the size of a logical volume.
- lvremove: This command removes a logical volume.
- pvdisplay: This command displays information about the physical volumes.
- vgdisplay: This command displays information about the volume groups.
- lvdisplay: This command displays information about the logical volumes.

Using LVM, you can create complex storage configurations, such as adding disks to extend a volume group, and then extending a logical volume to use that space. The benefits of using LVM include greater flexibility, ease of management, and the ability to resize partitions on the fly without having to unmount any filesystems. 

## tldr 
 
> Manage physical volumes, volume groups, and logical volumes using the Logical Volume Manager (LVM) interactive shell.
> More information: <https://man7.org/linux/man-pages/man8/lvm.8.html>.

- Start the Logical Volume Manager interactive shell:

`sudo lvm`

- List the Logical Volume Manager commands:

`sudo lvm help`

- Initialize a drive or partition to be used as a physical volume:

`sudo lvm pvcreate {{/dev/sdXY}}`

- Display information about physical volumes:

`sudo lvm pvdisplay`

- Create a volume group called vg1 from the physical volume on `/dev/sdXY`:

`sudo lvm vgcreate {{vg1}} {{/dev/sdXY}}`

- Display information about volume groups:

`sudo lvm vgdisplay`

- Create a logical volume with size 10G from volume group vg1:

`sudo lvm lvcreate -L {{10G}} {{vg1}}`

- Display information about logical volumes:

`sudo lvm lvdisplay`
