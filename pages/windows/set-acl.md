# Set-Acl 
## chatgpt 
The Set-Acl cmdlet in PowerShell is used to modify access control lists (ACLs) on a file or a directory. ACLs determine the permissions that are granted to or denied from users or groups to the resources, such as files or folders.

The syntax for the Set-Acl cmdlet is as follows:

```
Set-Acl [-Path] <string[]> [-AclObject <Object>] [-Include <string[]>] [-Exclude <string[]>] [-Filter <string>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

Where:

- `-Path` specifies the path or paths to the files or directories that you want to modify the security settings for. This parameter accepts multiple values.
- `-AclObject` specifies a custom ACL object to apply to the specified file or directory.
- `-Include` and `-Exclude` specify an array of file or directory names to include or exclude from the operation.
- `-Filter` specifies a wildcard pattern to filter the files or directories in the `-Path` parameter.
- `-PassThru` returns the modified object(s).
- `-WhatIf` shows what would happen if the cmdlet runs. The cmdlet does not execute if this parameter is used.
- `-Confirm` prompts you for confirmation before executing the cmdlet.

To modify an ACL, you can use the `-Path` parameter with a path to the file or directory you want to modify the permissions, and use the `-AclObject` to specify a custom ACL that defines the access permissions. 

For example, to grant full control permission to a user named "John" for a file named "example.txt", you can use the following command:

```
Set-Acl -Path C:\example.txt -AclObject (New-Acl -AccessRule (New-Object System.Security.AccessControl.FileSystemAccessRule('John','FullControl','Allow')))
```

This command uses the New-Acl and New-Object cmdlets to create a new ACL and a new access rule that grants full control permission to the user "John". The Set-Acl cmdlet then applies this ACL to the file "example.txt". 

## tldr 
 
> Changes the security descriptor of a specified item, such as a file or a registry key.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.security/set-acl>.

- Copy a security descriptor from one file to another:

`$OriginAcl = Get-Acl -Path {{path\to\file}}; Set-Acl -Path {{path\to\file}} -AclObject $OriginAcl`

- Use the pipeline operator to pass a descriptor:

`Get-Acl -Path {{path\to\file}} | Set-Acl -Path {{path\to\file}}`
