# btrfs inspect-internal 
## chatgpt 
The `btrfs inspect-internal` command is a Btrfs-specific tool that enables internal inspection of the Btrfs filesystem. It allows users to inspect and troubleshoot inconsistencies and errors in the Btrfs filesystem's internal data structures.

When executed, the `btrfs inspect-internal` command displays a list of options that allow users to inspect various areas of the filesystem. These options include:

- `dump-super`: Displays the contents of the superblock, which contains important information about the Btrfs filesystem.
- `check-integrity`: Verifies the integrity of the Btrfs filesystem by checking for errors in data blocks, metadata, and trees.
- `dump-tree`: Displays the contents of a Btrfs filesystem tree, which contains pointers to other elements of the filesystem.
- `rescue-super`: Attempts to recover a damaged or corrupted superblock by restoring a backup copy from a different part of the filesystem.
- `dump-block-groups`: Displays information about the Btrfs filesystem's block groups, which are used to manage data and metadata allocation.

Overall, the `btrfs inspect-internal` command is a powerful tool for diagnosing problems in a Btrfs filesystem and recovering from errors. However, it should be used with caution, as some options may cause data loss if used improperly. It is recommended that users backup their data before using any `btrfs inspect-internal` options. 

## tldr 
 
> Query internal information of a btrfs filesystem.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-inspect-internal.html>.

- Print superblock's information:

`sudo btrfs inspect-internal dump-super {{path/to/partition}}`

- Print superblock's and all of its copies' information:

`sudo btrfs inspect-internal dump-super --all {{path/to/partition}}`

- Print filesystem's metadata information:

`sudo btrfs inspect-internal dump-tree {{path/to/partition}}`

- Print list of files in inode `n`-th:

`sudo btrfs inspect-internal inode-resolve {{n}} {{path/to/btrfs_mount}}`

- Print list of files at a given logical address:

`sudo btrfs inspect-internal logical-resolve {{logical_address}} {{path/to/btrfs_mount}}`

- Print stats of root, extent, csum and fs trees:

`sudo btrfs inspect-internal tree-stats {{path/to/partition}}`
