# trash 
## chatgpt 
As an AI language model, I cannot provide an actual command named "trash" as it is not a standard command in most operating systems like Windows, Linux, or macOS, nor a commonly used external command utility or software. 

However, "trash" might refer to the Trash or Recycle Bin, which are folders where deleted files are temporarily stored to give users the ability to recover them later on. Here are some possible detailed explanations for the command "trash":

- In macOS: "trash" is a macOS command line utility that moves files and directories to the Trash. It is part of the BSD core utilities package and can be used to delete files via Terminal or shell scripts. The syntax is as follows: `trash file1 [file2 ...]`
- In Linux: There is no standard Linux command called "trash," but there are several third-party utilities that mimic macOS's trash command, such as Trash-CLI, which provides a command-line interface to the freedesktop.org Trash specification. The command to install Trash-CLI in Ubuntu or Debian based systems would be `sudo apt install trash-cli`.
- In Windows: There is no built-in "trash" command in Windows, but Windows users can use the "Recycle Bin" to perform the same operation. To access the Recycle Bin, you can use `shell:RecycleBinFolder` as a command in the "Run" program, or navigate to it using File Explorer. To delete a file or folder in the Recycle Bin, you can simply right-click and select "Delete."


Note: Be careful when using any command or program to delete files or folders, as there might be no way of recovering them after emptied the trash or the recycle bin. Always double-check before executing the command, especially if working with important files. 

## tldr 
 
> A CLI for managing the trashcan / recycling bin.
> More information: <https://github.com/andreafrancia/trash-cli>.

- Delete a file and send it to the trash:

`trash {{path/to/file}}`

- List all files in the trash:

`trash-list`

- Interactively restore a file from the trash:

`trash-restore`

- Empty the trash:

`trash-empty`

- Permanently delete all files in the trash which are older than 10 days:

`trash-empty {{10}}`

- Remove all files in the trash, which match a specific blob pattern:

`trash-rm "{{*.o}}"`

- Remove all files with a specific original location:

`trash-rm {{/path/to/file_or_directory}}`
