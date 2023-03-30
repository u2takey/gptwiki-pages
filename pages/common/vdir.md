# vdir 
## chatgpt 
The "vdir" command stands for "verbose directory." It is a command used in the command-line interface of an operating system. 

When you execute the "vdir" command, it displays a detailed list of the files and directories present in the current directory. The list includes the files' names, permissions, ownership, size, date of creation, and other details.

The vdir command is often used in conjunction with other commands to perform operations on the files and directories listed. For example, you can redirect the output of the vdir command to a text file to create a directory listing.

Overall, the vdir command is useful when you need to quickly view detailed information about the files and directories in a directory without having to navigate to them one by one. 

## tldr 
 
> List directory contents.
> Drop-in replacement for `ls -l`.
> More information: <https://www.gnu.org/software/coreutils/vdir>.

- List files and directories in the current directory, one per line, with details:

`vdir`

- List with sizes displayed in human-readable units (KB, MB, GB):

`vdir -h`

- List including hidden files (starting with a dot):

`vdir -a`

- List files and directories sorting entries by size (largest first):

`vdir -S`

- List files and directories sorting entries by modification time (newest first):

`vdir -t`

- List grouping directories first:

`vdir --group-directories-first`

- Recursively list all files and directories in a specific directory:

`vdir --recursive {{path/to/directory}}`
