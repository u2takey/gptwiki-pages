# blkdiscard 
## chatgpt 
The `blkdiscard` command is a Linux utility that is used to discard (erase) the contents of a block device. It essentially tells the storage device to mark all blocks as free so that the data on the device can no longer be accessed. This command is commonly used for Solid State Drives (SSDs) and other flash-based storage devices.

The syntax of the `blkdiscard` command is:

```
blkdiscard [options] device_path
```

Here, `device_path` is the path to the block device that you want to discard.

Some of the common options used with the `blkdiscard` command are:

- `-f`: Forces the command to execute without prompting for confirmation.
- `-s`: Secure mode that writes zeros to the blocks before discarding them.

Once you run the `blkdiscard` command, it will discard all the data on the specified device, making the data unrecoverable. It is important to note that this command should be used with caution as it irreversibly destroys all data on the device. It is therefore recommended to take a backup of the important data before running the command. 

## tldr 
 
> Discards device sectors on storage devices. Useful for SSDs.
> More information: <https://manned.org/blkdiscard>.

- Discard all sectors on a device, removing all data:

`blkdiscard /dev/{{device}}`

- Securely discard all blocks on a device, removing all data:

`blkdiscard --secure /dev/{{device}}`

- Discard the first 100 MB of a device:

`blkdiscard --length {{100MB}} /dev/{{device}}`
