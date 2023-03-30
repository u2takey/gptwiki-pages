# e4defrag 
## chatgpt 
The command e4defrag is used to defragment a file system in Linux. It works specifically with the ext4 file system.

When files on a file system are created, modified, or deleted, they are often not stored in a contiguous block on the disk. This can lead to fragmentation, which slows down file access times as the disk head must skip around to access all the pieces of a file.

The e4defrag command is used to defragment the ext4 file system by moving fragmented files into contiguous blocks on the disk. This helps to improve file access times and overall system performance.

The e4defrag command can be used with several options, including:

- -c or --check: Checks for fragmentation but does not defragment.
- -v or --verbose: Shows progress while defragmenting.
- -f or --force: Forces e4defrag to run on a mounted file system (which is normally not recommended).
- -r or --really-force: Forces e4defrag to defragment even if it detects potential data loss.

It is important to note that defragmentation can be a time-consuming process and can put a heavy load on the disk. It is recommended to backup important data before running the e4defrag command. 

## tldr 
 
> Defragment an ext4 filesystem.
> More information: <https://manned.org/e4defrag>.

- Defragment the filesystem:

`e4defrag {{/dev/sdXN}}`

- See how fragmented a filesystem is:

`e4defrag -c {{/dev/sdXN}}`

- Print errors and the fragmentation count before and after each file:

`e4defrag -v {{/dev/sdXN}}`
