# zpool 
## chatgpt 
zpool is a command used in the Solaris and OpenZFS operating systems to manage storage pools. A storage pool is a group of physical storage devices, such as hard drives or solid-state drives, that are combined into a single logical unit. This allows users to create RAID-like configurations, allocate storage space, and manage data redundancy.

The zpool command allows users to create, destroy, and modify storage pools. It supports a variety of storage configurations, such as mirrored storage (where data is duplicated across multiple disks for redundancy), striped storage (where data is split across multiple disks for performance), and hybrid configurations (that offer both redundancy and performance). The command also allows users to view information about their storage pools, including their size, status, and health.

Some common zpool commands are:

- zpool create: creates a new storage pool.
- zpool destroy: deletes an existing storage pool.
- zpool add: adds a new disk to an existing storage pool.
- zpool remove: removes a disk from an existing storage pool.
- zpool status: displays information about the status of a storage pool.
- zpool scrub: scans the storage pool for errors and corrects them if possible.
- zpool list: displays a list of all the storage pools on the system.
- zpool import: imports a previously-exported storage pool.
- zpool export: exports a storage pool, making it available to other systems. 

In summary, the zpool command is a powerful tool for managing storage pools in Solaris and OpenZFS operating systems, allowing users to create, modify, and monitor storage configurations. 

## tldr 
 
> Manage ZFS pools.
> More information: <https://manned.org/zpool>.

- Show the configuration and status of all ZFS zpools:

`zpool status`

- Check a ZFS pool for errors (verifies the checksum of EVERY block). Very CPU and disk intensive:

`zpool scrub {{pool_name}}`

- List zpools available for import:

`zpool import`

- Import a zpool:

`zpool import {{pool_name}}`

- Export a zpool (unmount all filesystems):

`zpool export {{pool_name}}`

- Show the history of all pool operations:

`zpool history {{pool_name}}`

- Create a mirrored pool:

`zpool create {{pool_name}} mirror {{disk1}} {{disk2}} mirror {{disk3}} {{disk4}}`

- Add a cache (L2ARC) device to a zpool:

`zpool add {{pool_name}} cache {{cache_disk}}`
