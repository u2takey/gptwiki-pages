# stat 
## chatgpt 
The "stat" command is a built-in Linux command used to display the status or information about a file or file system. The command is used to retrieve the following information:

1. File type – whether it's a regular file, directory, link or a device file.
2. Size of the file in bytes, blocks, and the total number of blocks utilized by the file system
3. Permissions of the file (read, write or execute) for the owner, group, and other users.
4. The file's creation, modification, and last access time stamp
5. The ID of the user who owns the file, and the group that the file belongs to
6. The device status and file system information

The "stat" command can be used with the filename, the relative path or absolute path of the file, and it can also be used with wildcards to display information about a group of files at once. 

For example:

$ stat myfile.txt
This will display the status of the file "myfile.txt" 

$ stat /home/user/*
This will display the status of all the files in the home directory of the user.

Overall, the "stat" command can be very useful in troubleshooting problems with files and file systems on Linux systems. 

## tldr 
 
> Display file and filesystem information.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/stat-invocation.html>.

- Display properties about a specific file such as size, permissions, creation and access dates among others:

`stat {{path/to/file}}`

- Display properties about a specific file such as size, permissions, creation and access dates among others without labels:

`stat --terse {{path/to/file}}`

- Display information about the filesystem where a specific file is located:

`stat --file-system {{path/to/file}}`

- Show only octal file permissions:

`stat --format="%a %n" {{path/to/file}}`

- Show the owner and group of a specific file:

`stat --format="%U %G" {{path/to/file}}`

- Show the size of a specific file in bytes:

`stat --format="%s %n" {{path/to/file}}`
