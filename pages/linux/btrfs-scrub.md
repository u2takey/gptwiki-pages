# btrfs scrub 
## chatgpt 
The "btrfs scrub" command is used to detect and repair data errors on a Btrfs file system. This command initiates a scrubbing process which reads all the data on the file system and compares it against the checksums of the respective data blocks stored in the file system.

During the scrubbing process, Btrfs checks for any errors such as checksum mismatches, bad sectors, and other errors that may have occurred due to hardware failure or other issues. If any errors are detected, the scrubbing process will attempt to repair them.

The "btrfs scrub" command requires root privileges to run and can be executed on a mounted Btrfs file system. It is recommended to run this command periodically to ensure the integrity and health of the file system.

Overall, the "btrfs scrub" command is a useful tool for maintaining the health of a Btrfs file system and safeguarding data against potential errors or corruption. 

## tldr 
 
> Scrub btrfs filesystems to verify data integrity.
> It is recommended to run a scrub once a month.
> More information: <https://btrfs.readthedocs.io/en/latest/btrfs-scrub.html>.

- Start a scrub:

`sudo btrfs scrub start {{path/to/btrfs_mount}}`

- Show the status of an ongoing or last completed scrub:

`sudo btrfs scrub status {{path/to/btrfs_mount}}`

- Cancel an ongoing scrub:

`sudo btrfs scrub cancel {{path/to/btrfs_mount}}`

- Resume a previously cancelled scrub:

`sudo btrfs scrub resume {{path/to/btrfs_mount}}`

- Start a scrub, but wait until the scrub finishes before exiting:

`sudo btrfs scrub start -B {{path/to/btrfs_mount}}`

- Start a scrub in quiet mode (does not print errors or statistics):

`sudo btrfs scrub start -q {{path/to/btrfs_mount}}`
