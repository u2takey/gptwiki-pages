# trash-cli 
## chatgpt 
The "trash-cli" command is used in the Linux terminal to move files and directories to the trash instead of permanently deleting them. It is essentially a command-line interface for the trash feature in Linux.

When you use the "trash-cli" command, it will move the specified file or directory to the trash folder. By default, the trash folder is located in the user's home directory and is hidden. You can access it by using the command "cd ~/.local/share/Trash/files".

The "trash-cli" command has several options:

1. "-r" or "--recursive": This option is used to move a directory to the trash.

2. "-f" or "--force": This option is used to forcefully move a file or directory to the trash without prompting for confirmation.

3. "-n" or "--no-interactive": This option is used to disable the interactive mode, i.e., it will not prompt for confirmation before moving the file or directory to the trash.

4. "-v" or "--verbose": This option is used to display verbose output, i.e., it will display more detailed information about the files or directories that are moved to the trash.

Overall, the "trash-cli" command is a useful command-line tool for safely deleting files and directories in Linux systems, especially if you want to avoid accidentally permanently deleting important files. 

## tldr 
 
> A command-line interface to the trashcan APIs.
> More information: <https://github.com/andreafrancia/trash-cli>.

- Trash specific files and directories into the current trashcan:

`trash-put {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Remove specific files from the current trashcan:

`trash-rm {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Empty the current trashcan:

`trash-empty`

- List trashed files and directories in the current trashcan:

`trash-list`

- Restore a specific file or directory by a number from the displayed list from the current trashcan:

`trash-restore`
