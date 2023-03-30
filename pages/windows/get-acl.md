# Get-Acl 
## chatgpt 
The Get-Acl command is a PowerShell cmdlet used to retrieve the Access Control List (ACL) for a specific file or directory. ACL provides a security mechanism for controlling access to files and folders by setting permissions for different users and groups.

When executed, the Get-Acl command returns a list of security descriptors for the specified items. This list includes the owner and group of the file or directory, as well as the individual permissions assigned to users and groups.

The syntax for the Get-Acl command is as follows:

Get-Acl [[-Path] <String[]>] [-LiteralPath <String[]>] [-Filter <String>] [-Include <String[]>] [-Exclude <String[]>] [-UseTransaction] [<CommonParameters>]

Where:

-Path: Specifies the path of the file or directory for which the ACL is to be retrieved.

-LiteralPath: Specifies the literal path of the file or directory, instead of interpreting it as a wildcard pattern.

-Filter: Specifies a wildcard pattern to filter the files or directories whose ACLs are to be retrieved.

-Include: Specifies an array of items to include in the results.

-Exclude: Specifies an array of items to exclude from the results.

-UseTransaction: Allows the command to be executed as part of a transaction.

<CommonParameters>: Specifies optional parameters that can be used with any cmdlet, such as Debug, Verbose, and ErrorAction.

Overall, the Get-Acl command is a useful tool for retrieving security information for files and directories, especially in a Windows environment. 

## tldr 
 
> Gets the security descriptor for a resource, such as a file or registry key.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.security/get-acl>.

- Display the ACL for a specific directory:

`Get-Acl {{path\to\directory}}`

- Get an ACL for a registry key:

`Get-Acl -Path {{HKLM:\System\CurrentControlSet\Control}} | Format-List`
