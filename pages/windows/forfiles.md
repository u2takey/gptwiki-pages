# forfiles 
## chatgpt 
Forfiles is a command in Windows operating system that is used to search for files and perform a specified command on them. It is typically used in batch files, command scripts, and command prompt.

The syntax of the forfiles command is as follows:

forfiles [/p <Path>] [/m <SearchMask>] [/s] [/c "<Command>"] [/d <Date>] 

The various options available with the forfiles command are:

/p: This option specifies the path of the file(s) that you want to search for. If this option is not specified, the search is done in the current directory.

/m: This option specifies the search mask for the file name. For example, if you want to search for all the text files, you can specify "/m *.txt".

/s: This option is used to search subdirectories as well. If this option is not specified, only the files in the specified directory are searched.

/c: This option is used to specify the command that you want to perform on the files that are found. The command can be any valid command that can be executed from the command prompt. For example, if you want to delete all the files that are found, you can specify "/c del @file"

/@file: This parameter is used by forfiles to substitute the filenames that are found by the search with @file.

/d: This option is used to specify the date range for the files that are searched. For example, if you want to search for files that were last modified in the last 7 days, you can specify "/d -7".

Overall, the forfiles command is a powerful tool for searching and performing batch operations on files and directories in Windows. 

## tldr 
 
> Select one or more files to execute a specified command on.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/forfiles>.

- Search for files in the current directory:

`forfiles`

- Search for files in a specific directory:

`forfiles /p {{path\to\directory}}`

- Run the specified command for each file:

`forfiles /c "{{command}}"`

- Search for files using a specific glob mask:

`forfiles /m {{glob_pattern}}`

- Search for files recursively:

`forfiles /s`

- Search for files older than 5 days:

`forfiles /d +{{5}}`
