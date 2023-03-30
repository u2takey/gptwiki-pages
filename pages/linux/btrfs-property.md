# btrfs property 
## chatgpt 
The "btrfs property" command is used to view or modify file system properties for a Btrfs file system. It provides a way to manage attributes of a file system such as compression, quota, and subvolume settings. 

Here are some of the common options and syntax for this command:

- To view all the available properties, you can simply type "btrfs property". 

- To view the current value of a specific property, use the "--get" option followed by the name of the property. For example, "btrfs property --get compression" will show you the current compression level of the file system.

- To set or change a specific property, use the "--set" option followed by the name of the property and its new value. For example, "btrfs property --set compression lzo" will change the compression level to LZO.

- Some properties may require additional parameters or options, such as the "quota" property that allows you to set usage limits for subvolumes. In this case, you would use the "--set" option followed by "quota" and the option(s) to specify the limits.

It's important to note that changing some properties may require the file system to be unmounted first, so always double-check the documentation or man page before making any modifications. 

## tldr 
 
> Get, set, or list properties for a given btrfs filesystem object (files, directories, subvolumes, filesystems, or devices).
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-property.html>.

- List available properties (and descriptions) for the given btrfs object:

`sudo btrfs property list {{path/to/btrfs_object}}`

- Get all properties for the given btrfs object:

`sudo btrfs property get {{path/to/btrfs_object}}`

- Get the `label` property for the given btrfs filesystem or device:

`sudo btrfs property get {{path/to/btrfs_filesystem}} label`

- Get all object type-specific properties for the given btrfs filesystem or device:

`sudo btrfs property get -t {{subvol|filesystem|inode|device}} {{path/to/btrfs_filesystem}}`

- Set the `compression` property for a given btrfs inode (either a file or directory):

`sudo btrfs property set {{path/to/btrfs_inode}} compression {{zstd|zlib|lzo|none}}`
