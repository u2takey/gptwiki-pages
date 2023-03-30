# robocopy 
## chatgpt 
Robocopy (Robust File Copy) is a command-line tool provided by Microsoft that allows for the copying of files and folders between locations.

The basic syntax of the "robocopy" command is as follows:

`robocopy [source] [destination] [file(s)] [options]`

- `[source]` is the location of the files to be copied.
- `[destination]` is the location where the files are to be copied.
- `[file(s)]` are the names of the files to be copied (optional).
- `[options]` are various parameters that modify the behavior and output of the command.

Some popular options for Robocopy are:

- `/E` - copy subdirectories including empty ones
- `/R:n` - number of times to retry if a file cannot be copied (default is 1 million)
- `/W:n` - wait time in seconds between retries (default is 30)
- `/ETA` - estimated time of completion
- `/Z` - copy files in restartable mode (for unreliable connections)
- `/MT[:n]` - use multi-threaded copying, where `n` is the number of threads (default is 8)

For example, to copy all files and subdirectories from the "C:\Users\Username\Documents" folder to the "D:\Backup" folder, while using multi-threaded copying with 16 threads, the following command can be used:

`robocopy C:\Users\Username\Documents D:\Backup /E /MT:16` 

## tldr 
 
> Robust File and Folder Copy.
> By default files will only be copied if the source and destination have different time stamps or different file sizes.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/robocopy>.

- Copy all `.jpg` and `.bmp` files from one directory to another:

`robocopy {{path\to\source_directory}} {{path\to\destination_directory}} {{*.jpg}} {{*.bmp}}`

- Copy all files and subdirectories, including empty ones:

`robocopy {{path\to\source_directory}} {{path\to\destination_directory}} /E`

- Mirror/Sync a directory, deleting anything not in source and include all attributes and permissions:

`robocopy {{path\to\source_directory}} {{path\to\destination_directory}} /MIR /COPYALL`

- Copy all files and subdirectories, excluding source files that are older than destination files:

`robocopy {{path\to\source_directory}} {{path\to\destination_directory}} /E /XO`

- List all files 50 MB or larger instead of copying them:

`robocopy {{path\to\source_directory}} {{path\to\destination_directory}} /MIN:{{52428800}} /L`

- Allow resuming if network connection is lost and limit retries to 5 and wait time to 15 sec:

`robocopy {{path\to\source_directory}} {{path\to\destination_directory}} /Z /R:5 /W:15`

- Display detailed usage information:

`robocopy /?`
