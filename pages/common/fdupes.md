# fdupes 
## chatgpt 
The "fdupes" command is a Linux utility used for finding and removing duplicate files in a directory. It scans the specified directory and detects any duplicate files by comparing their content, size, and modification time. 

The command syntax for fdupes is:

fdupes [OPTIONS] [DIRECTORY]

where OPTIONS are the various flags that modify the behavior of the command, and DIRECTORY is the path of the directory to be scanned. 

Some of the commonly used options for fdupes command are:

-d: Enables delete mode, allowing fdupes to automatically delete duplicate files.

-r: Recursively scans all subdirectories of the specified directory.

-n: Enables the no-prompt mode, which automatically deletes all duplicate files without asking for confirmation.

-S: Enables symlink follow mode, meaning it follows symbolic links in the specified directory.

-f: Enables the hard link detection mode, meaning it detects and reports hard links between files. 

The output of the fdupes command lists all the duplicate files found in the specified directory along with their path. It also displays the file size and the modification time of each file to help identify the duplicate files. 

Overall, the fdupes command is a useful tool for freeing up disk space by removing unnecessary duplicate files. 

## tldr 
 
> Finds duplicate files in a given set of directories.
> More information: <https://github.com/adrianlopezroche/fdupes>.

- Search a single directory:

`fdupes {{path/to/directory}}`

- Search multiple directories:

`fdupes {{directory1}} {{directory2}}`

- Search a directory recursively:

`fdupes -r {{path/to/directory}}`

- Search multiple directories, one recursively:

`fdupes {{directory1}} -R {{directory2}}`

- Search recursively and replace duplicates with hardlinks:

`fdupes -rH {{path/to/directory}}`

- Search recursively for duplicates and display interactive prompt to pick which ones to keep, deleting the others:

`fdupes -rd {{path/to/directory}}`

- Search recursively and delete duplicates without prompting:

`fdupes -rdN {{path/to/directory}}`
