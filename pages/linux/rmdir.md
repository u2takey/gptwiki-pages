# rmdir 
## chatgpt 
The command "rmdir" is used in command-line interface to remove or delete an empty directory. 

The command is typically used in the following format: 

rmdir [option] directory_name

Options:
- "-p" or "--parents": this option removes the parent directories as well if they are also empty.
- "-v" or "--verbose": this option shows the output of each directory being removed.

Directory_name is the name of the directory you want to remove.

When executed, this command will delete the specified directory if it is empty. If the directory contains files or subdirectories, the command will fail and an error message will be displayed. It's important to note that the "rmdir" command cannot be used to delete directories with files or subdirectories, and it's recommended to use the "rm -r" command instead. 

## tldr 
 
> Remove directories without files.
> See also: `rm`.
> More information: <https://www.gnu.org/software/coreutils/rmdir>.

- Remove specific directories:

`rmdir {{path/to/directory1 path/to/directory2 ...}}`

- Remove specific nested directories recursively:

`rmdir --parents {{path/to/directory1 path/to/directory2 ...}}`
