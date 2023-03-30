# udisksctl 
## chatgpt 
The `udisksctl` command is a command-line tool for interacting with disks and storage devices on Linux systems using the `udisksd` daemon. It allows users to perform various operations related to managing and interacting with storage devices.

The `udisksctl` command can be used to list all available storage devices, mount/unmount partitions, format disks, check the file system on disks, and perform other disk management tasks.

Here are some of the common options and usage examples for the `udisksctl` command:

- `list`: List all available disks and partitions.
```
$ udisksctl list
```

- `info`: Get detailed information about a specific device or partition.
```
$ udisksctl info /dev/sda1
```

- `mount`: Mount a partition to a specified mount point.
```
$ udisksctl mount -b /dev/sda1
```

- `unmount`: Unmount a partition.
```
$ udisksctl unmount -b /dev/sda1
```

- `format`: Format a disk with a specified file system.
```
$ udisksctl format -f ext4 /dev/sda
```

Overall, the `udisksctl` command provides a convenient and powerful way to manage storage devices on Linux systems. 

## tldr 
 
> A command-line program used to interact with the udisksd daemon process.
> More information: <http://storaged.org/doc/udisks2-api/latest/udisksctl.1.html>.

- Show high-level information about disk drives and block devices:

`udisksctl status`

- Show detailed information about a device:

`udisksctl info --block-device {{/dev/sdX}}`

- Show detailed information about a device partition:

`udisksctl info --block-device {{/dev/sdXN}}`

- Mount a device partition and prints the mount point:

`udisksctl mount --block-device {{/dev/sdXN}}`

- Unmount a device partition:

`udisksctl unmount --block-device {{/dev/sdXN}}`

- Monitor the daemon for events:

`udisksctl monitor`
