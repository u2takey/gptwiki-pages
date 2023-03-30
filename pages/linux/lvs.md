# lvs 
## chatgpt 
The `lvs` command is used in Linux to display detailed information about logical volume groups (VG), logical volumes (LV) and their properties. It is a part of the LVM (Logical Volume Manager) system which allows dynamic storage allocation and maintenance.

When the `lvs` command is executed, it displays the following information by default:

- LV Path: The full path of the logical volume
- LV Name: The name of the logical volume
- VG Name: The name of the volume group
- LV UUID: Unique identifier of the logical volume
- LV Size: The size of the logical volume
- LV Status: The operational status of the logical volume
- LV Open: The number of processes currently accessing the logical volume

Additional information, such as the number of allocated and free extents, and the type of filesystem used, can be displayed by using different options with the `lvs` command.

Some of the commonly used options with the `lvs` command are:

- `-a`: Display all the logical volumes including hidden and inactive ones
- `-o`: Specify the columns to display
- `-S`: Filter the output based on specified conditions
- `-v`: Display more verbose output, such as major and minor device numbers and kernel driver in use

Overall, the `lvs` command is a powerful tool for managing and monitoring storage in a Linux system. 

## tldr 
 
> Display information about logical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvs.8.html>.

- Display information about logical volumes:

`lvs`

- Display all logical volumes:

`lvs -a`

- Change default display to show more details:

`lvs -v`

- Display only specific fields:

`lvs -o {{field_name_1}},{{field_name_2}}`

- Append field to default display:

`lvs -o +{{field_name}}`

- Suppress heading line:

`lvs --noheadings`

- Use a separator to separate fields:

`lvs --separator {{=}}`
