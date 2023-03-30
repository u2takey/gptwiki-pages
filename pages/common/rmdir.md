# rmdir 
## chatgpt 
The rmdir command, short for "remove directory", is a command typically used in command line interfaces to delete empty directories in a file system. 

Syntax:
rmdir [options] <directory>

Options:
The options vary slightly depending on the operating system being used, but some commonly used options include:
- -p, --parents: Removes the parent directories as well if they become empty after removing a subdirectory.
- -v, --verbose: Shows a message for each directory that is removed.
- -h, --help: Displays the help menu for the command.

Directory:
This is the name of the directory to be removed. The directory should be an absolute or relative path name to the directory to be deleted.

Note: 
It is important to note that the rmdir command can only remove empty directories. If the directory still contains files, subdirectories or any other items, it will not be deleted. In such cases, you'll have to use the rm command with the -r or -R option to delete the directory and its contents recursively. 

Example:
To delete an empty directory named "testdir", you can use the following command:
rmdir testdir

If the directory is not empty, you can remove it recursively including all of its files and sub-directories as follows:
rm -r /path/to/directory 

## tldr 
 
> Remove directories without files.
> See also: `rm`.
> More information: <https://www.gnu.org/software/coreutils/rmdir>.

- Remove specific directories:

`rmdir {{path/to/directory1 path/to/directory2 ...}}`

- Remove specific nested directories recursively:

`rmdir -p {{path/to/directory1 path/to/directory2 ...}}`
