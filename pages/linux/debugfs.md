# debugfs 
## chatgpt 
The "debugfs" command is a Linux utility that provides advanced debugging features for the file system. It is used to troubleshoot and debug file system-related problems.

Here's a detailed explanation of some common options used with the debugfs command:

- `-c`: This option creates a new filesystem on the specified device. It formats the device and creates a new file system superblock.

- `-w`: This option allows write access to the filesystem. With this option, you can update, change or delete files, directories, and other file system attributes.

- `-R`: This option allows you to run a series of Debugger commands before entering the interactive mode. You can run multiple commands by separating them with semicolons.

- `-f`: This option reads file system commands from the specified file instead of entering the interactive mode.

Using debugfs, you can perform various operations such as browsing the file system, viewing and editing file system attributes, modifying and deleting files and directories, repairing file system corruption, etc.

However, the debugfs command should be used with caution as it is designed for advanced users and can cause data loss if used improperly. It is recommended to take a backup of your file system before using debugfs. 

## tldr 
 
> An interactive ext2/ext3/ext4 filesystem debugger.
> More information: <https://manned.org/debugfs>.

- Open the filesystem in read only mode:

`debugfs {{/dev/sdXN}}`

- Open the filesystem in read write mode:

`debugfs -w {{/dev/sdXN}}`

- Read commands from a specified file, execute them and then exit:

`debugfs -f {{path/to/cmd_file}} {{/dev/sdXN}}`

- View the filesystem stats in debugfs console:

`stats`

- Close the filesystem:

`close -a`

- List all available commands:

`lr`
