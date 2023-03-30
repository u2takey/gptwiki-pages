# Resolve-Path 
## chatgpt 
The Resolve-Path is a PowerShell cmdlet that is used to resolve a specified path. It is used to convert a relative path or a partial path to an absolute path in the PowerShell.

The Resolve-Path command essentially takes a string input that represents a path and returns the resolved absolute path of that input. This absolute path is based on the current location of the user in the file system and can include symbolic links or variables. This command is especially useful when working with variables or relative paths in PowerShell.

For example, if the current location of the user in the file system is "C:\Users\John\Documents" and the input path is "files\test.txt", Resolve-Path will return the resolved absolute path of the file "C:\Users\John\Documents\files\test.txt".

The Resolve-Path command also supports multiple path inputs, which can be specified as an array. This allows the command to resolve multiple paths at once, making it more efficient when working with multiple files.

In summary, the Resolve-Path command is used to resolve a specified path and return the absolute path of that input based on the user's current location in the file system. 

## tldr 
 
> Resolves the wildcard characters in a path, and displays the path contents.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.management/resolve-path>.

- Resolve the home folder path:

`Resolve-Path {{~}}`

- Resolve a UNC path:

`Resolve-Path -Path "\\{{hostname}}\{{path\to\file}}"`

- Get relative paths:

`Resolve-Path -Path {{path\to\file_or_directory}} -Relative`
