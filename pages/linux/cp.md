# cp 
## chatgpt 
The cp command is used in Linux/Unix operating systems to copy files and directories from a source location to a destination location. It stands for 'copy'. Here's a breakdown of the command's syntax and some options that can be used:

Syntax: 

cp [options] source_file(destination_file)

Options:

- -r: Recursively copies a directory and its contents
- -i: Interactive mode, prompting the user before overwriting files
- -u: Copies only files that are newer than the destination file
- -f: Forces copy operation, overwriting existing files without prompting

Examples:

1. To copy a file from one directory to another, we'll use the following syntax: 

cp /path/to/source/file /path/to/destination/folder

2. To copy a directory and all its contents, we use the '-r' option:

cp -r /path/to/source/directory /path/to/destination/directory

3. To copy multiple files at once, list them all as arguments after the source and destination:

cp file1 file2 /path/to/destination/

In summary, the cp command is a versatile way to copy files and directories, with several options to customize the copying operation. 

## tldr 
 
> Copy files and directories.
> More information: <https://www.gnu.org/software/coreutils/cp>.

- Copy a file to another location:

`cp {{path/to/source_file.ext}} {{path/to/target_file.ext}}`

- Copy a file into another directory, keeping the filename:

`cp {{path/to/source_file.ext}} {{path/to/target_parent_directory}}`

- Recursively copy a directory's contents to another location (if the destination exists, the directory is copied inside it):

`cp -r {{path/to/source_directory}} {{path/to/target_directory}}`

- Copy a directory recursively, in verbose mode (shows files as they are copied):

`cp -vr {{path/to/source_directory}} {{path/to/target_directory}}`

- Copy text files to another location, in interactive mode (prompts user before overwriting):

`cp -i {{*.txt}} {{path/to/target_directory}}`

- Follow symbolic links before copying:

`cp -L {{link}} {{path/to/target_directory}}`

- Use the full path of source files, creating any missing intermediate directories when copying:

`cp --parents {{source/path/to/file}} {{path/to/target_file}}`
