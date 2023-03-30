# pmount 
## chatgpt 
The `pmount` command is a command-line tool for mounting removable USB drives, CD-ROMs, and other mass storage devices. The command is used to mount a file system on a removable device onto a specified directory in the file system hierarchy.

When executed, `pmount` prompts the user for the device partition to mount, as well as the mount point. It then mounts the device to the specified mount point, allowing the user to browse and manipulate the files on the device. 

The advantage of using `pmount` over other mounting tools is that it does not require root privileges, making it a safer option for mounting removable mass storage devices. 

The `pmount` command also supports the use of options, such as `-r` for read-only access and `-f` to force the file system to be mounted. 

Overall, `pmount` provides a convenient and secure way to mount removable mass storage devices in a Linux operating system. 

## tldr 
 
> Mount arbitrary hotpluggable devices as a normal user.
> More information: <https://manned.org/pmount>.

- Mount a device below `/media/` (using device as mount point):

`pmount {{/dev/to/block/device}}`

- Mount a device with a specific filesystem type to `/media/label`:

`pmount --type {{filesystem}} {{/dev/to/block/device}} {{label}}`

- Mount a CD-ROM (filesystem type ISO9660) in read-only mode:

`pmount --type {{iso9660}} --read-only {{/dev/cdrom}}`

- Mount an NTFS-formatted disk, forcing read-write access:

`pmount --type {{ntfs}} --read-write {{/dev/sdX}}`

- Display all mounted removable devices:

`pmount`
