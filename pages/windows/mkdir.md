# mkdir 
## chatgpt 
The "mkdir" command is a command-line utility in Linux and other Unix-based operating systems that allows users to create new directories or folders in a specified location. The name stands for "make directory."

To use the "mkdir" command, users need to open a terminal or command prompt and type "mkdir" followed by a space and the desired name(s) of the new directories. For example, to create a new directory called "myfolder" in the current working directory, you would type:

mkdir myfolder

If you want to create multiple directories at once, separate the names with a space:

mkdir dir1 dir2 dir3

You can also create multiple directories within a single command using the "-p" option, which allows you to create a nested directory structure. For example, to create a directory called "myfolder" inside a directory called "parentfolder" that does not yet exist, you would type:

mkdir -p parentfolder/myfolder

The "-p" option ensures that both the parent directory and the new subdirectory are created at once, rather than returning an error if the parent directory does not already exist.

By default, "mkdir" creates new directories with read, write, and execute permissions for the user who created them, but no permissions for anyone else. Users can use the "chmod" command to modify the permissions of a directory after it has been created. 

## tldr 
 
> Creates a directory.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/mkdir>.

- Create a directory:

`mkdir {{path\to\directory}}`

- Create a nested directory tree recursively:

`mkdir {{path\to\sub_directory}}`
