# pvs 
## chatgpt 
The "pvs" command in Linux is used to display volume group (VG) and physical volume (PV) information. It is a part of the LVM (Logical Volume Management) toolset and can be used to provide information about the available disks or partitions, allocated space on each disk, and the overall size of the disk.

When you run the "pvs" command, it will display the following information:

- Physical volume name: This indicates the name of the physical volume that the information pertains to.
- Volume group name: This shows the name of the volume group that the physical volume is a part of.
- PV size: This is the total size of the physical volume.
- PV free: This shows the amount of free space available on the physical volume.
- PV used: This is the amount of space that is currently being used on the physical volume.
- PV UUID: This is the universally unique identifier of the physical volume.

Additionally, the output from the "pvs" command may also include flags or other indicators that show the status of the physical volume, such as whether it is active or inactive.

Overall, the "pvs" command is a useful tool for managing volumes in Linux, especially when used in combination with other LVM commands. 

## tldr 
 
> Display information about physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvs.8.html>.

- Display information about physical volumes:

`pvs`

- Display non-physical volumes:

`pvs -a`

- Change default display to show more details:

`pvs -v`

- Display only specific fields:

`pvs -o {{field_name_1}},{{field_name_2}}`

- Append field to default display:

`pvs -o +{{field_name}}`

- Suppress heading line:

`pvs --noheadings`

- Use separator to separate fields:

`pvs --separator {{special_character}}`
