# dir 
## chatgpt 
The "dir" command is a Windows command which tells the computer to display a list of all the files and directories in the current directory. It shows the name, size, date modified and other information about each file and directory. The command is primarily used to quickly view or list files and directories within a specific directory. The command can also be used with some parameters or switches, such as to sort by size, date or type, or to display only hidden files or directories. The command can be executed in the Command Prompt or in Windows PowerShell. 

## tldr 
 
> List directory contents using one line per file, special characters are represented by backslash escape sequences.
> Works as `ls -C --escape`.
> More information: <https://manned.org/dir>.

- List all files, including hidden files:

`dir -all`

- List files including their author (`-l` is required):

`dir -l --author`

- List files excluding those that match a specified blob pattern:

`dir --hide={{pattern}}`

- List subdirectories recursively:

`dir --recursive`

- Display help:

`dir --help`
