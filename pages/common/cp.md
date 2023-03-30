# cp 
## chatgpt 
The cp command is a Linux command that is used to copy files or directories from one location to another location. It stands for "copy".

The basic syntax of the cp command is as follows:

cp [options] source_file destination

Here is what each part of the command means:

- cp: this is the command itself, telling the system to copy a file or directory.
- [options]: there are several options that can be used with the cp command, such as -r for copying directories recursively, -f for forcing the copy even if the destination file already exists, or -p for preserving the original file metadata.
- source_file: this is the file or directory that you want to copy.
- destination: this is the location where you want to copy the file or directory.

For example, to copy a file called "file1.txt" from the current working directory to the /home/user/ directory, you would use the following command:

cp file1.txt /home/user/

Alternatively, if you wanted to copy an entire directory called "directory1" and all of its contents to /home/user/directory2, you would use the following command:

cp -r directory1 /home/user/directory2

This would copy the directory recursively ("-r" option) and create a new directory called "directory1" inside the destination directory ("directory2"). 

## tldr 
 
> Copy files and directories.
> More information: <https://www.gnu.org/software/coreutils/cp>.

- Copy a file to another location:

`cp {{path/to/source_file.ext}} {{path/to/target_file.ext}}`

- Copy a file into another directory, keeping the filename:

`cp {{path/to/source_file.ext}} {{path/to/target_parent_directory}}`

- Recursively copy a directory's contents to another location (if the destination exists, the directory is copied inside it):

`cp -R {{path/to/source_directory}} {{path/to/target_directory}}`

- Copy a directory recursively, in verbose mode (shows files as they are copied):

`cp -vR {{path/to/source_directory}} {{path/to/target_directory}}`

- Copy text files to another location, in interactive mode (prompts user before overwriting):

`cp -i {{*.txt}} {{path/to/target_directory}}`

- Follow symbolic links before copying:

`cp -L {{link}} {{path/to/target_directory}}`

- Use the first argument as the destination directory (useful for `xargs ... | cp -t <DEST_DIR>`):

`cp -t {{path/to/target_directory}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`
