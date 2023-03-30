# where 
## chatgpt 
The command "where" is a command used in command-line interfaces to find the location(s) of a specific executable file. 

When a user types a command on the command-line prompt, the shell checks if the command is an executable file located in one of the directories in the system's PATH environment variable. If the command is found, the shell executes it. If it is not found, the shell throws an error.

The "where" command is used to search for the location of a command or executable file. It displays the paths of all the files that match the searched name. By default, the "where" command searches for files in the current directory and the directories listed in the system's PATH environment variable.

The syntax for the "where" command is:

```
where <filename>
```

For example, to find the location of the "notepad.exe" in the system, the user can type:

```
where notepad.exe
```

The command will display the paths of all the files named "notepad.exe" that are located in the directories that are accessible from the current command prompt.

The "where" command is available in most command-line interfaces, including Windows Command Prompt, PowerShell, and Unix-based terminal shells. It is particularly useful for identifying the locations of executable files that are part of the system or installed applications. 

## tldr 
 
> This command is an alias of `Where-Object`.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.core/where-object>.

- View documentation for the original command:

`tldr Where-Object`
