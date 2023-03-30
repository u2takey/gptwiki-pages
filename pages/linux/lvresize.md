# lvresize 
## chatgpt 
The “lvresize” command is a Linux command used to resize a logical volume within a physical volume. It is typically used to change the size of the logical volume, either by increasing or decreasing its size. The command must be run as a superuser or with sudo privileges.

The syntax of the lvresize command is as follows:

lvresize [OPTIONS] LogVolPath [SIZE]

Where:

- [OPTIONS]: optional flags that can modify the behavior of the command.
- LogVolPath: the path to the logical volume that needs to be resized.
- [SIZE]: optional target size for the logical volume.

Some common options for the lvresize command include:

- -L, --size : Used to specify the new size of the logical volume.
- -r, --resizefs: Used to automatically resize the file system to match the new size of the logical volume.

When running the lvresize command, the logical volume must be unmounted before it can be resized. If the file system on the logical volume is mounted, it can cause data corruption and other issues. If the file system on the logical volume is not mounted, you can use the "-r" option to automatically resize the file system. Otherwise, you can resize the file system manually after resizing the logical volume.

Overall, the lvresize command is a useful tool for managing logical volumes on a Linux system, allowing you to easily resize them as needed. 

## tldr 
 
> Change the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvresize.8.html>.

- Change the size of a logical volume to 120 GB:

`lvresize --size {{120G}} {{volume_group}}/{{logical_volume}}`

- Extend the size of a logical volume as well as the underlying filesystem by 120 GB:

`lvresize --size +{{120G}} --resizefs {{volume_group}}/{{logical_volume}}`

- Extend the size of a logical volume to 100% of the free physical volume space:

`lvresize --size {{100}}%FREE {{volume_group}}/{{logical_volume}}`

- Reduce the size of a logical volume as well as the underlying filesystem by 120 GB:

`lvresize --size -{{120G}} --resizefs {{volume_group}}/{{logical_volume}}`
