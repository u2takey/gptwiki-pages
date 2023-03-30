# df 
## chatgpt 
The "df" command stands for "disk free" and is used in Unix-based operating systems to display information about the file system's disk space usage.

When executed, the "df" command displays the following information in columns:
- The file system's device name or location
- The total size of the file system in kilobytes (KB), megabytes (MB), or gigabytes (GB)
- The amount of used space in kilobytes, megabytes or gigabytes
- The amount of free space in kilobytes, megabytes or gigabytes
- The percentage of disk space that is currently used by the file system
- The file system's mount point (where it is attached to the operating system's file hierarchy)

The "df" command is typically used with options such as "-h" to display the sizes in a more human-readable format (such as "GB" instead of "kilobytes"), "-T" to include the file system's type, or "-i" to display the number of used and free inodes (the data structure used to store information about the files and directories).

Overall, "df" is a useful command for checking the disk space usage of a file system and identifying potential issues with disk space availability. 

## tldr 
 
> Gives an overview of the filesystem disk space usage.
> More information: <https://www.gnu.org/software/coreutils/df>.

- Display all filesystems and their disk usage:

`df`

- Display all filesystems and their disk usage in human-readable form:

`df -h`

- Display the filesystem and its disk usage containing the given file or directory:

`df {{path/to/file_or_directory}}`

- Display statistics on the number of free inodes:

`df -i`

- Display filesystems but exclude the specified types:

`df -x {{squashfs}} -x {{tmpfs}}`
