# chmod 
## chatgpt 
The chmod command is a Linux/Unix command that is used to change permissions of files and directories. 

The syntax of the chmod command is as follows: 

`chmod [options] mode file(s)`

Here, [options] are the various options that can be used with the chmod command, mode is the new mode or permission that you want to set for the file or directory, and file(s) is the file or directory whose permission you want to change. 

Some of the commonly used options with the chmod command are: 

- `-r`: changes the permission recursively for all files and sub-directories within a directory
- `-v`: displays the changes made to files and directories
- `-c`: displays a message only if a file's permission is changed

The mode parameter in the chmod command specifies the new permission that you want to set for the file or directory. It can be specified in three different ways: 

- Numeric mode: This consists of three numbers that represent read, write, and execute permissions. For example, 777 represents full permission for the owner, group, and others.
- Symbolic mode: This involves using symbols such as +, -, and = in combination with letters r, w, and x to specify permission changes. For example, `chmod u+rw myfile` adds read and write permission for the owner of the file.
- Absolute mode: This is a combination of numeric and symbolic mode, where you can specify permission for each category of users (owner, group, and others) separately. For example, `chmod 644 myfile` sets read and write permission for the owner and read permission for group and others.

In summary, the chmod command is a powerful tool for changing file and directory permissions in Linux/Unix operating systems. It enables users to set or modify permission settings in various ways, depending on their needs. 

## tldr 
 
> Change the access permissions of a file or directory.
> More information: <https://www.gnu.org/software/coreutils/chmod>.

- Give the [u]ser who owns a file the right to e[x]ecute it:

`chmod u+x {{path/to/file}}`

- Give the [u]ser rights to [r]ead and [w]rite to a file/directory:

`chmod u+rw {{path/to/file_or_directory}}`

- Remove e[x]ecutable rights from the [g]roup:

`chmod g-x {{path/to/file}}`

- Give [a]ll users rights to [r]ead and e[x]ecute:

`chmod a+rx {{path/to/file}}`

- Give [o]thers (not in the file owner's group) the same rights as the [g]roup:

`chmod o=g {{path/to/file}}`

- Remove all rights from [o]thers:

`chmod o= {{path/to/file}}`

- Change permissions recursively giving [g]roup and [o]thers the ability to [w]rite:

`chmod -R g+w,o+w {{path/to/directory}}`

- Recursively give [a]ll users [r]ead permissions to files and e[X]ecute permissions to sub-directories within a directory:

`chmod -R a+rX {{path/to/directory}}`
