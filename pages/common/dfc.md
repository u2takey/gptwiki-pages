# dfc 
## chatgpt 
The `dfc` command is used to display disk space usage information in a colorful and easy-to-read format. It is an alternative to the traditional `df` command which can be difficult to read and understand if you have multiple storage devices mounted on your system.

When you run the `dfc` command in your terminal, it will display a table containing the following information about each mounted file system:

- File system name
- Type of file system
- Total size of the file system
- Used space in the file system
- Free space in the file system
- Percentage of disk space used
- Mount point

The command is mainly used to quickly view the disk usage statistics of file systems on your machine. It provides an easy-to-read output that allows you to quickly identify which file systems are running low on space.

The `dfc` command is not installed by default on most Linux distributions. You will need to install it either via your distribution's package manager or via manually downloading and installing the package.

Overall, the `dfc` command provides a quick and easy way to get an overview of your disk usage at a glance. 

## tldr 
 
> Gives an overview of the filesystem disk space usage with colors and graphs.
> More information: <https://projects.gw-computing.net/projects/dfc/wiki>.

- Display filesystems and their disk usage in human-readable form with colors and graphs:

`dfc`

- Display all filesystems including pseudo, duplicate and inaccessible filesystems:

`dfc -a`

- Display filesystems without color:

`dfc -c never`

- Display filesystems containing "ext" in the filesystem type:

`dfc -t ext`
