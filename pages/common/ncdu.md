# ncdu 
## chatgpt 
ncdu is a command line utility for analyzing disk usage. It stands for NCurses Disk Usage, as it allows for a user-friendly interface through the use of the ncurses library. 

When executed, ncdu starts by scanning the current directory and all subdirectories, gathering statistics on file and directory sizes. It then presents this information in a navigable and interactive interface, which allows a user to browse through the directories and see how much space is being used by each file or folder.

Some of the features of ncdu include the ability to sort files and directories by size, delete selected files, and export usage reports in different formats. It can be particularly useful for identifying large, unnecessary files or directories that can be removed to free up disk space.
 
Overall, ncdu is an easy-to-use and powerful tool for managing disk space usage on Linux systems. 

## tldr 
 
> Disk usage analyzer with an ncurses interface.
> More information: <https://manned.org/ncdu>.

- Analyze the current working directory:

`ncdu`

- Colorize output:

`ncdu --color {{dark|off}}`

- Analyze a given directory:

`ncdu {{path/to/directory}}`

- Save results to a file:

`ncdu -o {{path/to/file}}`

- Exclude files that match a pattern, argument can be given multiple times to add more patterns:

`ncdu --exclude '{{*.txt}}'`
