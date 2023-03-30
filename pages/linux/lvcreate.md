# lvcreate 
## chatgpt 
The "lvcreate" command is used in Linux to create a new logical volume. Logical volumes are used as virtual partitions within a physical disk, which are then used to store data. The lvcreate command allows the user to specify various parameters such as the name of the logical volume, its size, and its location on the physical disk.

Syntax:
The syntax of the lvcreate command is as follows: 

lvcreate [options] VG LUN 

Where: 
- “options” are the various additional parameters
- “VG” is the volume group name to which the logical volume belongs to  
- “LUN” is the logical unit name that has to be created. 

Options:
Some of the common options used with the lvcreate command are: 

- -L: Specifies the size of the logical volume in units like KB, MB, GB, etc.
- -n: Specifies the name of the logical volume to be created.
- -y: Skips the confirmation prompt, automatically confirms the LV creation.
- -Z: Zeros out a space on disk to create additional space for LV creation.
- -r: Specifies which file system should be integrated with the new logical volume.
- --nameprefixes: Add a prefix to a logical volume name.

Example:
To create a new logical volume of size 16G with the name "lv_data" in the volume group "vg00," you can use the following command:

lvcreate -L 16G -n lv_data vg00

This command will create a new logical volume of size 16 GB in the "vg00" volume group with the logical volume named "lv_data." 

Note:
- You must have permission to create and modify files on the target drive.
- It's always best practice to backup your data before performing any disk operation. 

## tldr 
 
> Creates a logical volume in an existing volume group. A volume group is a collection of logical and physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvcreate.8.html>.

- Create a logical volume of 10 gigabytes in the volume group vg1:

`lvcreate -L {{10G}} {{vg1}}`

- Create a 1500 megabyte linear logical volume named mylv in the volume group vg1:

`lvcreate -L {{1500}} -n {{mylv}} {{vg1}}`

- Create a logical volume called mylv that uses 60% of the total space in volume group vg1:

`lvcreate -l {{60%VG}} -n {{mylv}} {{vg1}}`

- Create a logical volume called mylv that uses all the unallocated space in the volume group vg1:

`lvcreate -l {{100%FREE}} -n {{mylv}} {{vg1}}`
