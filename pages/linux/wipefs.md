# wipefs 
## chatgpt 
The `wipefs` command is a Linux utility that is used to erase different types of file system signatures, boot signatures, and disk labels from a storage device. The command is typically used to remove any existing file system signature or partition table from a device. When the command is executed, it reads and erases the first sectors of a storage device or file and then removes any existing signatures from that device.

Here is an example of how the `wipefs` command is used:

```
sudo wipefs /dev/sdb
```

In this example, the `wipefs` command is used to erase any existing file system or partition table from the `/dev/sdb` device. The `sudo` command is used to execute the command with root privileges. 

The `wipefs` command can also be used to delete individual file system signatures or specific signatures from a storage device. The following command shows how to delete a specific signature from the device `/dev/sdb1`:

```
sudo wipefs -t ext4 /dev/sdb1
```

In this example, the `-t` option is used to specify the file system type and the `ext4` argument is used to specify the file system type to be erased.

Overall, the `wipefs` command is a powerful tool for erasing file system signatures and partition tables from storage devices in Linux systems. However, it should be used with caution as it can completely wipe out all data on a device if misused. 

## tldr 
 
> Wipe filesystem, raid, or partition-table signatures from a device.
> More information: <https://manned.org/wipefs>.

- Display signatures for specified device:

`sudo wipefs {{/dev/sdX}}`

- Wipe all available signature types for a specific device with no recursion into partitions:

`sudo wipefs --all {{/dev/sdX}}`

- Wipe all available signature types for the device and partitions using a glob pattern:

`sudo wipefs --all {{/dev/sdX}}*`

- Perform dry run:

`sudo wipefs --all --no-act {{/dev/sdX}}`

- Force wipe, even if the filesystem is mounted:

`sudo wipefs --all --force {{/dev/sdX}}`
