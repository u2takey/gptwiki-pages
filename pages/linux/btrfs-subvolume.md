# btrfs subvolume 
## chatgpt 
The `btrfs subvolume` command is used in the Btrfs file system to control subvolumes, which are logical partitions within the file system that act like separate file systems. 

Here are some of the most common options and subcommands used with `btrfs subvolume`:

- `create`: This subcommand is used to create a new subvolume. For example, `btrfs subvolume create /mnt/btrfs/test_subvol` would create a new subvolume called "test_subvol" in the /mnt/btrfs directory.
- `delete`: This subcommand is used to delete a subvolume. For example, `btrfs subvolume delete /mnt/btrfs/test_subvol` would delete the subvolume called "test_subvol" in the /mnt/btrfs directory.
- `snapshot`: This subcommand is used to create a snapshot of a subvolume. A snapshot is a read-only copy of a subvolume that can be used for backups or as a point-in-time reference. For example, `btrfs subvolume snapshot /mnt/btrfs/test_subvol /mnt/btrfs/test_subvol_snapshot` would create a snapshot of the "test_subvol" subvolume called "test_subvol_snapshot" in the /mnt/btrfs directory.
- `list`: This subcommand is used to list all subvolumes. For example, `btrfs subvolume list /mnt/btrfs` would list all subvolumes in the /mnt/btrfs directory.
- `show`: This subcommand is used to display information about a specific subvolume. For example, `btrfs subvolume show /mnt/btrfs/test_subvol` would display information about the "test_subvol" subvolume. 

## tldr 
 
> Manage btrfs subvolumes and snapshots.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-subvolume.html>.

- Create a new empty subvolume:

`sudo btrfs subvolume create {{path/to/new_subvolume}}`

- List all subvolumes and snapshots in the specified filesystem:

`sudo btrfs subvolume list {{path/to/btrfs_filesystem}}`

- Delete a subvolume:

`sudo btrfs subvolume delete {{path/to/subvolume}}`

- Create a read-only snapshot of an existing subvolume:

`sudo btrfs subvolume snapshot -r {{path/to/source_subvolume}} {{path/to/target}}`

- Create a read-write snapshot of an existing subvolume:

`sudo btrfs subvolume snapshot {{path/to/source_subvolume}} {{path/to/target}}`

- Show detailed information about a subvolume:

`sudo btrfs subvolume show {{path/to/subvolume}}`
