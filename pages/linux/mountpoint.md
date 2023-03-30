# mountpoint 
## chatgpt 
The `mountpoint` command is used to determine whether or not a directory is a mount point. A mount point is a directory that acts as an access point for a file system. When a file system is mounted, it is attached to a mount point and becomes accessible to the user.

When used with the name of a directory as an argument, the `mountpoint` command will return one of two values: 0 or 1. A return value of 0 indicates that the directory is a mount point, while a return value of 1 indicates that it is not.

The `mountpoint` command can also be used with the `-q` or `--quiet` option to suppress output, and the `-d` or `--device` option to specify the device to check for a mount point.

Overall, the `mountpoint` command is useful for determining whether or not a file system is currently mounted, and can be used in scripts and automation tasks to make decisions based on the current state of the system. 

## tldr 
 
> Test if a directory is a filesystem mountpoint.
> More information: <https://manned.org/mountpoint>.

- Check if a directory is a mountpoint:

`mountpoint {{path/to/directory}}`

- Check if a directory is a mountpoint without showing any output:

`mountpoint -q {{path/to/directory}}`

- Show major/minor numbers of a mountpoint's filesystem:

`mountpoint --fs-devno {{path/to/directory}}`
