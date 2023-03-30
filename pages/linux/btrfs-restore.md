# btrfs restore 
## chatgpt 
The "btrfs restore" command is used in Linux-based operating systems for the purpose of recovering data from a corrupted Btrfs file system. Here is a detailed explanation of this command:

- "btrfs": This is the name of the file system type that the command is designed to work with. Btrfs, which stands for "B-tree file system," is a modern file system that is optimized for scalability, reliability, and data integrity. It is commonly used in Linux-based operating systems for storage management.

- "restore": This is the action that the command performs. When you run "btrfs restore," you are instructing the system to recover data from a corrupted Btrfs file system.

To use "btrfs restore," you typically need to provide certain parameters and options along with the command. Here are some of the most common ones:

- "-v": This option enables verbose mode, which provides more detailed information about the restore process.

- "-t": This option specifies the point-in-time from which you want to restore data. You can provide a specific timestamp or a range of dates and times.

- "-D": This option instructs the system to restore deleted files as well as existing ones.

- "-r": This option enables read-only mode, which prevents the system from making any changes to the restored data.

- "destination": This is the path where you want the restored data to be saved. You can specify a directory path or a file path.

Here's an example of how you might use "btrfs restore" to recover data from a corrupted Btrfs file system:

btrfs restore -v -t "2022-01-01 10:00" -D -r /mnt/mydata-backup/ /mnt/mydata-restored/

In this example, we are asking the system to restore data from the "/mnt/mydata-backup/" directory that was backed up on January 1st, 2022 at 10:00 AM. We also want the system to restore any deleted files and save the restored data to "/mnt/mydata-restored/". The "-v" option will provide us with more detailed information about the restore process, while the "-r" option will prevent the system from making any changes to the original backup data. 

## tldr 
 
> Try to salvage files from a damaged btrfs filesystem.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-restore.html>.

- Restore all files from a btrfs filesystem to a given directory:

`sudo btrfs restore {{path/to/btrfs_device}} {{path/to/target_directory}}`

- List (don't write) files to be restored from a btrfs filesystem:

`sudo btrfs restore --dry-run {{path/to/btrfs_device}} {{path/to/target_directory}}`

- Restore files matching a given regex ([c]ase-insensitive) files to be restored from a btrfs filesystem (all parent directories of target file(s) must match as well):

`sudo btrfs restore --path-regex {{regex}} -c {{path/to/btrfs_device}} {{path/to/target_directory}}`

- Restore files from a btrfs filesystem using a specific root tree `bytenr` (see `btrfs-find-root`):

`sudo btrfs restore -t {{bytenr}} {{path/to/btrfs_device}} {{path/to/target_directory}}`

- Restore files from a btrfs filesystem (along with metadata, extended attributes, and Symlinks), overwriting files in the target:

`sudo btrfs restore --metadata --xattr --symlinks --overwrite {{path/to/btrfs_device}} {{path/to/target_directory}}`
