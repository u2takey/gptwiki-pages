# btrfs device 
## chatgpt 
The `btrfs device` command is a sub-command used in the Btrfs file system on Linux systems. This command is used to manage physical devices in Btrfs, such as adding or removing devices to or from a Btrfs filesystem.

The `btrfs device` command supports various options and sub-commands, some of which are:

- `add`: This option is used to add a new device to the Btrfs filesystem. For example, `btrfs device add /dev/sdb /mnt/btrfs` will add a new device `/dev/sdb` to the existing Btrfs filesystem mounted at `/mnt/btrfs`.
- `delete`: This option is used to remove a device from the Btrfs filesystem. For example, `btrfs device delete /dev/sdc /mnt/btrfs` will remove the device `/dev/sdc` from the Btrfs filesystem mounted at `/mnt/btrfs`.
- `scan`: This option is used to scan for new devices that can be added to the Btrfs filesystem. For example, `btrfs device scan` will scan the system for new devices that can be added to the Btrfs filesystem.
- `show`: This option is used to display information about the devices in the Btrfs filesystem. For example, `btrfs device show /mnt/btrfs` will display information about the devices used in the Btrfs filesystem mounted at `/mnt/btrfs`.

In summary, the `btrfs device` command is used to manage physical devices in a Btrfs filesystem, including adding, removing, scanning, and displaying information about these devices. 

## tldr 
 
> Manage devices in a btrfs filesystem.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-device.html>.

- Add one or more devices to a btrfs filesystem:

`sudo btrfs device add {{path/to/block_device1}} [{{path/to/block_device2}}] {{path/to/btrfs_filesystem}}`

- Remove a device from a btrfs filesystem:

`sudo btrfs device remove {{path/to/device|device_id}} [{{...}}]`

- Display error statistics:

`sudo btrfs device stats {{path/to/btrfs_filesystem}}`

- Scan all disks and inform the kernel of all detected btrfs filesystems:

`sudo btrfs device scan --all-devices`

- Display detailed per-disk allocation statistics:

`sudo btrfs device usage {{path/to/btrfs_filesystem}}`
