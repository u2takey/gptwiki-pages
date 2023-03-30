# chown 
## chatgpt 
The "chown" command is a Unix command that stands for "change owner." It is used to change the ownership of a file or directory in a Unix-based operating system, such as Linux or Mac OS.

The syntax for the chown command is as follows:

```
chown [OPTIONS] [OWNER][:[GROUP]] FILE
```

Where:

- `OPTIONS` are any additional arguments you want to pass to the command. Some of the most common options include `-R` (recursively change ownership of all files and directories within a directory), `-v` (verbose output), and `-h` (change the ownership of symbolic links).
- `OWNER` is the new owner of the file or directory. This can be either a username (e.g. "john") or a user ID (e.g. "1234").
- `GROUP` is the new group owner of the file or directory. This is optional, and if omitted, the file or directory will retain its current group ownership.

For example, to change the owner of the file "file.txt" to the user "john", you would run the following command:

```
chown john file.txt
```

To change the ownership of all files and directories within the directory "my_folder" to the user "john" and the group "admins", you would run the following command:

```
chown -R john:admins my_folder
```

It is important to note that only the current owner of a file or directory or the root user can change the ownership of a file or directory. Additionally, changing the ownership of system files or directories can potentially break the functionality of the system, so it should be done with caution. 

## tldr 
 
> Change user and group ownership of files and directories.
> More information: <https://www.gnu.org/software/coreutils/chown>.

- Change the owner user of a file/directory:

`chown {{user}} {{path/to/file_or_directory}}`

- Change the owner user and group of a file/directory:

`chown {{user}}:{{group}} {{path/to/file_or_directory}}`

- Recursively change the owner of a directory and its contents:

`chown -R {{user}} {{path/to/directory}}`

- Change the owner of a symbolic link:

`chown -h {{user}} {{path/to/symlink}}`

- Change the owner of a file/directory to match a reference file:

`chown --reference={{path/to/reference_file}} {{path/to/file_or_directory}}`
