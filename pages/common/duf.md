# duf 
## chatgpt 
The "duf" command refers to Disk Usage Free utility, which is a command-line tool that displays the disk usage statistics for all partitions and mount points in a human-readable format. It is an alternative to the "du" command, which is a built-in tool in Unix-like systems used to analyze file size and disk usage.

When the "duf" command is run in a terminal, it quickly provides a summary of the disk usage statistics for all the filesystems available.  Here are some of the features of the "duf" command:

- It shows disk usage information in a clear and easy-to-read format.
- Displays the total size, percentage of usage, available space, and the number of files and directories for each mount point or partition.
- The output can be sorted by any column to help identify which directories consuming the most space.
- It supports keyboard shortcuts to easily navigate through the output.
- The color-coded output makes it easy to identify directories with the most usage.

Example usage:

To use the "duf" command, simply enter "duf" in the command line on a terminal, followed by pressing enter. This will display the summary of disk usage statistics for all available partitions/mount points. Optionally, you can add the path to the directory that you want to analyze to see the usage statistics for just that specific directory.

For example, to check disk usage statistics for the "/usr" directory, you can use the following command:

```
duf /usr
```
The above command will display the disk usage statistics for the "/usr" directory. 

## tldr 
 
> Disk Usage/Free Utility.
> More information: <https://github.com/muesli/duf>.

- List accessible devices:

`duf`

- List everything (such as pseudo, duplicate or inaccessible file systems):

`duf --all`

- Only show specified devices or mount points:

`duf {{path/to/directory1 path/to/directory2 ...}}`

- Sort the output by a specified criteria:

`duf --sort {{size|used|avail|usage}}`
