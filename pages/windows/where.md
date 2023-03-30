# where 
## chatgpt 
The command "where" is a Windows command-line tool used to locate the location of an executable file or command. When you enter a command in the command prompt, Windows searches through the directories listed in the PATH environment variable to find the location of the command's executable file.

The "where" command can be used to find the exact path of the executable file of a command, including any aliases or alternative names. This can be useful in troubleshooting issues with missing or conflicting files, or when you need to know which version of a command you are using.

To use the "where" command, open a command prompt and type "where" followed by the name of the command you want to locate. For example, "where notepad" will show you the exact path of the Notepad executable file.

You can also use wildcards like "*" or "?" to search for a specific set of commands. For example, "where dir*" will display all executable files that start with "dir".

Overall, the "where" command can be a powerful tool for navigating and troubleshooting the command prompt. 

## tldr 
 
> Display the location of files that match the search pattern.
> Defaults to current work directory and paths in the PATH environment variable.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/where>.

- Display the location of file pattern:

`where {{file_pattern}}`

- Display the location of file pattern including file size and date:

`where /T {{file_pattern}}`

- Recursively search for file pattern at specified path:

`where /R {{path\to\directory}} {{file_pattern}}`

- Silently return the error code for the location of the file pattern:

`where /Q {{file_pattern}}`
