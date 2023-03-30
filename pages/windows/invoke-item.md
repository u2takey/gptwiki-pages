# Invoke-Item 
## chatgpt 
The command "Invoke-Item" is used in PowerShell to open or execute a file, folder or application. It can be used with a file path, UNC path or with a variable that contains the file path. 

Syntax: 

Invoke-Item [-Path] <String[]> [-Credential <PSCredential>] [-UseTransaction] [<CommonParameters>]

Here, 

-Path: Specifies the path to the file, folder or application to be opened or executed.

-Credential: Specifies the user account credentials to use to perform the operation. 

-UseTransaction: Includes the operation in the active transaction.

CommonParameters: This cmdlet supports the common parameters: Verbose, Debug, ErrorAction, ErrorVariable, WarningAction, WarningVariable, OutBuffer, PipelineVariable, and OutVariable. 

Examples:

1. To open a file in PowerShell:
Invoke-Item "C:\Users\user1\Documents\file.txt"

2. To open an application in PowerShell:
Invoke-Item "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe"

3. To open a folder in PowerShell:
Invoke-Item "C:\Users\user1\Documents"

4. To open a file using a variable:
$path = "C:\Users\user1\Documents\file.txt"
Invoke-Item $path

In summary, the "Invoke-Item" command is used to open or execute a file, folder or application in PowerShell. 

## tldr 
 
> Open files in their respective default programs.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.management/invoke-item>.

- Open a file in its default program:

`Invoke-Item -Path {{path\to\file}}`

- Open all files inside a directory:

`Invoke-Item -Path {{path\to\directory}}\*`

- Open all PNGs inside a directory:

`Invoke-Item -Path {{path\to\directory}}\*.png`

- Open all files inside a directory containing a specific keyword:

`Invoke-Item -Path {{path\to\directory}}\* -Include {{*keyword*}}`

- Open all files inside a directory except those containing a specific keyword:

`Invoke-Item -Path {{path\to\directory}}\* -Exclude {{*keyword*}}`

- Perform a dry run to determine which files will be opened inside a directory through `Invoke-Item`:

`Invoke-Item -Path {{path\to\directory}}\* -WhatIf`
