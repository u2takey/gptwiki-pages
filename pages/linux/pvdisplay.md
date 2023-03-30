# pvdisplay 
## chatgpt 
The `pvdisplay` command is used to display the physical volume information of a LVM partition. It stands for "physical volume display". Here's what each part of the command means:

- `pvdisplay`: This is the actual command that you're running. It tells the system to display the physical volume information.

When you run the `pvdisplay` command, it will typically display the following information for each physical volume:

- Physical Volume Name: This is the name of the physical volume (or volumes) that are being displayed.
- VG Name: This is the name of the volume group that the physical volume is a part of.
- PV Size: This is the size of the physical volume.
- Allocatable: This indicates whether or not the physical volume is currently allocated.
- PE Size: This is the size of each physical extent (PE) on the physical volume.
- Total PE: This is the total number of physical extents on the physical volume.
- Free PE: This is the number of unallocated physical extents on the physical volume.
- PV UUID: This is a unique identifier for the physical volume.

Overall, the `pvdisplay` command is a useful tool for viewing information about the physical volumes that are currently in use on a Linux system. 

## tldr 
 
> Display information about Logical Volume Manager (LVM) physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvdisplay.8.html>.

- Display information about all physical volumes:

`sudo pvdisplay`

- Display information about the physical volume on drive `/dev/sdXY`:

`sudo pvdisplay {{/dev/sdXY}}`
