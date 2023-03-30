# extundelete 
## chatgpt 
extundelete is a command-line tool used to recover deleted files and directories from EXT3 or EXT4 partitions. It works by scanning the file system's journal to determine which files were deleted and then attempts to recover them.

The basic syntax for using extundelete is:

extundelete [OPTIONS] DEVICE

Here, DEVICE refers to the block device or file system image from which the deleted files are to be recovered.

Some of the common options that can be used with extundelete are:

- --restore-all: Recover all deleted files and directories.
- --restore-file FILENAME: Recover a specific file with the specified name.
- --restore-directory PATH: Recover all files and directories contained in the specified directory.
- --output-dir DIRECTORY: Specify the directory where recovered files should be stored.
- --inode INODE: Recover a file by specifying its inode number.
- --after TIME: Recover files deleted after the specified time.
- --before TIME: Recover files deleted before the specified time.
- --version: Show the version of extundelete.

It is important to note that extundelete should be used with caution, as it may not be able to recover all deleted files and there is a risk of overwriting other data on the file system. Additionally, it should be used immediately after data loss to increase the chances of recovery. 

## tldr 
 
> Recover deleted files from ext3 or ext4 partitions by parsing the journal.
> See also `date` for Unix time information and `umount` for unmounting partitions.
> More information: <http://extundelete.sourceforge.net>.

- Restore all deleted files inside partition N on device X:

`sudo extundelete {{/dev/sdXN}} --restore-all`

- Restore a file from a path relative to root (Do not start the path with `/`):

`extundelete {{/dev/sdXN}} --restore-file {{path/to/file}}`

- Restore a directory from a path relative to root (Do not start the path with `/`):

`extundelete {{/dev/sdXN}} --restore-directory {{path/to/directory}}`

- Restore all files deleted after January 1st, 2020 (in Unix time):

`extundelete {{/dev/sdXN}} --restore-all --after {{1577840400}}`
