# zfs 
## chatgpt 
ZFS (Zettabyte File System) is a high-performance file system designed for large-scale storage systems. It provides a robust, reliable, and scalable solution for managing large amounts of data. ZFS file system has many advanced features such as support for multiple disk pools, automatic data compression, data deduplication, and snapshot management.

The ZFS command is used to create, manage, and administer ZFS file systems. The command is used to manage ZFS storage pools, datasets, snapshots, and clones. It is typically used from the command line, and can be executed with options and arguments to perform various actions on ZFS file systems.

Some of the common ZFS commands are:

- zfs create: This command is used to create a new ZFS file system or dataset.
- zfs destroy: This command is used to destroy a ZFS file system or dataset.
- zfs list: This command is used to display information about ZFS file systems and datasets.
- zfs snapshot: This command is used to create a read-only snapshot of a ZFS file system or dataset.
- zfs send: This command is used to send a ZFS snapshot to another system or device.
- zfs receive: This command is used to receive a ZFS snapshot from another system or device.

Overall, the ZFS command provides a powerful set of tools for managing ZFS file systems and datasets, and is an essential tool for anyone working with large-scale storage systems. 

## tldr 
 
> Manage ZFS filesystems.
> More information: <https://manned.org/zfs>.

- List all available zfs filesystems:

`zfs list`

- Create a new ZFS filesystem:

`zfs create {{pool_name/filesystem_name}}`

- Delete a ZFS filesystem:

`zfs destroy {{pool_name/filesystem_name}}`

- Create a Snapshot of a ZFS filesystem:

`zfs snapshot {{pool_name/filesystem_name}}@{{snapshot_name}}`

- Enable compression on a filesystem:

`zfs set compression=on {{pool_name/filesystem_name}}`

- Change mountpoint for a filesystem:

`zfs set mountpoint={{/my/mount/path}} {{pool_name/filesystem_name}}`
