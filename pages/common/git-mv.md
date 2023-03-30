# git mv 
## chatgpt 
The "git mv" command in Git is used to move or rename a file or directory in a repository. It is used to reflect the changes made to the structure of the project at any point in time. This command can move or rename any files or directories to a new path.

The syntax for the "git mv" command is:

$ git mv <source_file_path> <destination_file_path>

This command will rename the file or directory specified in the source path by the new name at the destination path. If the destination file path is not provided, Git will rename the file or directory with the same name.

The "git mv" command not only renames the file or directory but also stages the changes to be committed. This means that the changes will not be committed until the user manually commits the changes.

Additionally, the "git mv" command will track the move and history of the file. This means that Git will remember the changes and the history of the file or directory even after they have been moved or renamed.

Overall, the "git mv" command is used to rename or move files and directories in a Git repository while preserving its history and tracking its changes. 

## tldr 
 
> Move or rename files and update the Git index.
> More information: <https://git-scm.com/docs/git-mv>.

- Move file inside the repo and add the movement to the next commit:

`git mv {{path/to/file}} {{new/path/to/file}}`

- Rename file and add renaming to the next commit:

`git mv {{filename}} {{new_filename}}`

- Overwrite the file in the target path if it exists:

`git mv --force {{file}} {{target}}`
