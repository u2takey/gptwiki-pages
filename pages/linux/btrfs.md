# btrfs 
## chatgpt 
Btrfs is a command-line utility for creating and managing Btrfs filesystems. Btrfs (B-tree file system) is a modern copy-on-write file system that's designed for Linux-based operating systems. It's essentially a replacement for the traditional file systems like ext4 and XFS.

Some of the features of Btrfs include:

- Ability to create snapshots and roll back changes
- Support for creating subvolumes (a mechanism for logically dividing a single file system)
- Data checksumming for improved integrity
- Easy resizing of file systems on the fly

Here are some Btrfs commands and their explanations:

- `mkfs.btrfs`: This command creates a new Btrfs filesystem on a given disk or partition. For example, to create a new Btrfs file system on a partition called /dev/sda1, the command would be `mkfs.btrfs /dev/sda1`

- `btrfs subvolume create`: This command creates a new subvolume within an existing Btrfs filesystem. You can create a subvolume for a specific purpose, such as storing your music or photos. For example, `btrfs subvolume create /mnt/btrfs/photos` will create a "photos" subvolume in the Btrfs file system mounted at /mnt/btrfs.

- `btrfs subvolume snapshot`: This command creates a read-only snapshot of a subvolume. Snapshots are useful for creating backups or testing purposes. For example, `btrfs subvolume snapshot /mnt/btrfs/photos /mnt/btrfs/photos-backup` will create a read-only snapshot of the "photos" subvolume.

- `btrfs send` and `btrfs receive`: These commands are used for sending and receiving incremental backups of a Btrfs file system. You can use them to create backups of subvolumes or the entire file system. For example, `btrfs send /mnt/btrfs/photos | ssh user@backuphost "btrfs receive /mnt/backup/btrfs/photos"` will send a backup of the "photos" subvolume over SSH to a remote host.

- `btrfs balance`: This command balances data between devices in a Btrfs file system to improve performance and avoid having devices that are more full than others. For example, `btrfs balance start /mnt/btrfs` will balance the data between all devices in the Btrfs file system mounted at /mnt/btrfs.

Overall, Btrfs is a powerful and flexible file system with many advanced features that can make it a great choice for Linux users. 

## tldr 
 
> A filesystem based on the copy-on-write (COW) principle for Linux.
> Some subcommands such as `btrfs device` have their own usage documentation.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs.html>.

- Create subvolume:

`sudo btrfs subvolume create {{path/to/subvolume}}`

- List subvolumes:

`sudo btrfs subvolume list {{path/to/mount_point}}`

- Show space usage information:

`sudo btrfs filesystem df {{path/to/mount_point}}`

- Enable quota:

`sudo btrfs quota enable {{path/to/subvolume}}`

- Show quota:

`sudo btrfs qgroup show {{path/to/subvolume}}`
