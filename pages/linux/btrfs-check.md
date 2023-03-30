# btrfs check 
## chatgpt 
The 'btrfs check' command is used to check the integrity of a Btrfs file system. This command can detect various types of corruption including missing or corrupted data, metadata errors, and tree or block errors.

By issuing the command 'btrfs check' without any additional options, it will perform an online check of the file system, which means that the file system can continue to be used during the check.

The command may also be used with additional options. For example, the '-p' flag can be used to check and repair the parity of RAID 5 and RAID 6 volumes. The '-r' flag enables read-only mode so that the command only reports errors without making changes to the file system.

Overall, the command 'btrfs check' is a useful tool for ensuring the integrity and reliability of a Btrfs file system. It is recommended to run this command periodically to maintain the health of the file system. 

## tldr 
 
> Check or repair a btrfs filesystem.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-check.html>.

- Check a btrfs filesystem:

`sudo btrfs check {{path/to/partition}}`

- Check and repair a btrfs filesystem (dangerous):

`sudo btrfs check --repair {{path/to/partition}}`

- Show the progress of the check:

`sudo btrfs check --progress {{path/to/partition}}`

- Verify the checksum of each data block (if the filesystem is good):

`sudo btrfs check --check-data-csum {{path/to/partition}}`

- Use the `n`-th superblock (`n` can be 0, 1 or 2):

`sudo btrfs check --super {{n}} {{path/to/partition}}`

- Rebuild the checksum tree:

`sudo btrfs check --repair --init-csum-tree {{path/to/partition}}`

- Rebuild the extent tree:

`sudo btrfs check --repair --init-extent-tree {{path/to/partition}}`
