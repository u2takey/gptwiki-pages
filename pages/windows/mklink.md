# mklink 
## chatgpt 
The command "mklink" is a command in Windows operating systems that creates symbolic links or hard links between files or directories.

Syntax: 

mklink /D "new_directory_link_path" "existing_directory_path"

mklink "new_file_link_path" "existing_file_path"

Options:

/D: specifies that the link is a directory symbolic link; otherwise, it creates a file symbolic link by default.

Examples:

1. To create a symbolic link for a folder named "Folder", located at C:\Users\Example\Documents\Folder, and link it to a new folder named "LinkFolder" at C:\Users\Example\Desktop\LinkFolder, you can use the following command:

mklink /D C:\Users\Example\Desktop\LinkFolder C:\Users\Example\Documents\Folder

2. To create a symbolic link for a file named "File.txt" located at C:\Users\Example\Documents\File.txt, and link it to a new file named "LinkFile.txt" at C:\Users\Example\Desktop\LinkFile.txt, you can use the following command:

mklink C:\Users\Example\Desktop\LinkFile.txt C:\Users\Example\Documents\File.txt

Note: The mklink command requires administrator privileges to execute. 

## tldr 
 
> Create symbolic links.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/mklink>.

- Create a symbolic link to a file:

`mklink {{path\to\link_file}} {{path\to\source_file}}`

- Create a symbolic link to a directory:

`mklink /d {{path\to\link_file}} {{path\to\source_directory}}`

- Create a hard link to a file:

`mklink /h {{path\to\link_file}} {{path\to\source_file}}`

- Create a directory junction:

`mklink /j {{path\to\link_file}} {{path\to\source_file}}`
