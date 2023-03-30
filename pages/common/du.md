# du 
## chatgpt 
The 'du' command in Unix/Linux stands for "disk usage" and is used to estimate and summarize the total space used by a specific file or directory, including its subdirectories. 

When executed, the 'du' command scans through the current working directory and reports the amount of disk space used by each file and directory in the output. It also displays the total size occupied by the parent directory.

The basic syntax of the 'du' command is:

    du [options] [directory/file name]
    
Some of the commonly used options are:

- -a: Display the sizes of all files and directories, including hidden files.
- -h: Print the output in a human-readable format (e.g., KB, MB, GB).
- -s: Display only the total size of the specified directory.
- -c: Display a grand total of the disk space used by multiple directories or files.

For example, running the command "du -h" in the terminal will display the disk usage of all files and directories in the current working directory in a human-readable format. To get disk usage of a specific directory, you can use the command "du -h /path/to/directory".

Overall, the 'du' command is useful for monitoring disk space usage and for identifying large files or directories that may be causing storage issues. 

## tldr 
 
> Disk usage: estimate and summarize file and directory space usage.
> More information: <https://www.gnu.org/software/coreutils/du>.

- List the sizes of a directory and any subdirectories, in the given unit (B/KiB/MiB):

`du -{{b|k|m}} {{path/to/directory}}`

- List the sizes of a directory and any subdirectories, in human-readable form (i.e. auto-selecting the appropriate unit for each size):

`du -h {{path/to/directory}}`

- Show the size of a single directory, in human-readable units:

`du -sh {{path/to/directory}}`

- List the human-readable sizes of a directory and of all the files and directories within it:

`du -ah {{path/to/directory}}`

- List the human-readable sizes of a directory and any subdirectories, up to N levels deep:

`du -h --max-depth=N {{path/to/directory}}`

- List the human-readable size of all `.jpg` files in subdirectories of the current directory, and show a cumulative total at the end:

`du -ch {{*/*.jpg}}`
