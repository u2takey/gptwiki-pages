# gdu 
## chatgpt 
The "gdu" command is a Linux utility that stands for "GNU Disk Usage". It is a command-line utility that allows you to view disk space usage data for a specified directory or file.

When you run the "gdu" command, it will scan the directory or file that you specify and display a report of the disk space usage. This report includes information such as the size of each file and directory, the percentage of disk space used by each file or directory, and the total size of the directory or file.

The "gdu" command also includes various options that allow you to customize the output of the report. For example, you can use the "--human-readable" option to display the sizes in a more easily readable format (such as "24 MB" instead of "24649600 bytes"). You can also use the "--exclude" option to specify files or directories that you want to exclude from the report.

Overall, the "gdu" command is a useful utility for managing disk space on a Linux system, as it allows you to quickly identify which files and directories are taking up the most space. 

## tldr 
 
> Disk usage analyzer with console interface.
> More information: <https://github.com/dundee/gdu>.

- Interactively show the disk usage of the current directory:

`gdu`

- Interactively show the disk usage of a given directory:

`gdu {{path/to/directory}}`

- Interactively show the disk usage of all mounted disks:

`gdu --show-disks`

- Interactively show the disk usage of the current directory but ignore some sub-directories:

`gdu --ignore-dirs {{path/to/directory1,path/to/directory2,...}}`

- Ignore paths by regular expression:

`gdu --ignore-dirs-pattern '{{.*[abc]+}}'`

- Ignore hidden directories:

`gdu --no-hidden`

- Only print the result, do not enter interactive mode:

`gdu --non-interactive {{path/to/directory}}`

- Do not show the progress in non-interactive mode (useful in scripts):

`gdu --no-progress {{path/to/directory}}`
