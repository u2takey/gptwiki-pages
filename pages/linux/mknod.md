# mknod 
## chatgpt 
The `mknod` command is used in Unix-based operating systems to create special files, also known as device nodes. These files provide a way for user programs to interact with hardware devices and system resources.

Syntax: `mknod [options] name type [major minor]`

Arguments:
- `name`: the name of the device node to create.
- `type`: the type of device node to create, either `b` for a block device or `c` for a character device.
- `major`: the major device number.
- `minor`: the minor device number.

Options:
- `-m`: set the file permissions on the newly created device node.
- `-g`: set the group ownership of the newly created device node.
- `-u`: set the user ownership of the newly created device node.

Example:
To create a block device node with major number `8` and minor number `0`, named `myblock`, in the current directory with permissions `0666`, one can use the following command:

```
mknod myblock b 8 0 -m 0666
```

This will create a block device file named `myblock` in the current directory, owned by the current user with permissions `0666`. Other programs can now use this file to interact with the block device it represents. 

## tldr 
 
> Create block or character device special files.
> More information: <https://www.gnu.org/software/coreutils/mknod>.

- Create a block device:

`sudo mknod {{path/to/device_file}} b {{major_device_number}} {{minor_device_number}}`

- Create a character device:

`sudo mknod {{path/to/device_file}} c {{major_device_number}} {{minor_device_number}}`

- Create a FIFO (queue) device:

`sudo mknod {{path/to/device_file}} p`

- Create a device file with default SELinux security context:

`sudo mknod -Z {{path/to/device_file}} {{type}} {{major_device_number}} {{minor_device_number}}`
