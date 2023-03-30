# Get-ChildItem 
## chatgpt 
The command "Get-ChildItem" is a PowerShell cmdlet used to display a list of files and folders in a specified directory. 

The syntax of the command is: 

Get-ChildItem [-Path] <String[]> [-Filter <String>] [-Include <String[]>] [-Exclude <String[]>] [-Recurse] [-Directory] [-File] [-Hidden] [-ReadOnly] [-System] [-Force] [-Credential <PSCredential>] [-UseTransaction] [<CommonParameters>]

Here's a breakdown of each parameter: 

- "-Path": Specifies the directory for which you want to retrieve the files and folders. This can be a local directory or a network share.
- "-Filter": Specifies the criteria used to filter the files and directories to be displayed.
- "-Include": Specifies the file extensions or directory names to be included in the output.
- "-Exclude": Specifies the file extensions or directory names to be excluded from the output.
- "-Recurse": Includes all subdirectories in the search.
- "-Directory" or "-File": Limits output to only directories or files respectively.
- "-Hidden" or "-ReadOnly" or "-System": Filters output based on file attributes.
- "-Force": Displays hidden and system files.
- "-Credential": Specifies backup operator or administrator credentials.
- "-UseTransaction": Commits changes as a single unit of work.

Once the command is executed, it returns a list of files and folders in the specified directory. The output includes the name, size, and last modified date of each file, as well as the name of each subdirectory. 

## tldr 
 
> List items in a directory.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.management/get-childitem>.

- List all non-hidden items in the current directory:

`Get-ChildItem`

- List only directories in the current directory:

`Get-ChildItem -Directory`

- List only files in the current directory:

`Get-ChildItem -File`

- List items in the current directory, including hidden items:

`Get-ChildItem -Hidden`

- List items in a directory other than the current one:

`Get-ChildItem -Path {{path\to\directory}}`
