# sls 
## chatgpt 
As an AI language model, I am not sure which context it is being referred to. However, I can give you a general explanation of the "sls" command.

The "sls" command is typically used in the Windows PowerShell environment. It stands for Select-String, which is a PowerShell cmdlet used to search for a specific string or pattern in a file or a set of files. 

The syntax for the "sls" command is:

sls [-Pattern] <string> [-Path] <string[]> [-Include <string[]>] [-Exclude <string[]>]
[-CaseSensitive] [-List] [-Quiet] [-SimpleMatch] [-AllMatches] [-Encoding <Encoding>]

Here are some examples of how to use the "sls" command:

1. To search for a string in a file:

sls "example" C:\Users\username\Documents\sample.txt

This will search for the string "example" in the file "sample.txt" located in the Documents folder of the user "username".

2. To search for a string in all the files in a folder and its subfolders:

sls "example" C:\Users\username\Desktop\myfolder\* -Recurse

This will search for the string "example" in all the files located in the "myfolder" folder on the Desktop of the user "username", including all subfolders.

3. To search for a string and display only the filenames:

sls "example" C:\Users\username\Desktop\myfolder\* -List

This will search for the string "example" in all files located in the "myfolder" folder on the Desktop of the user "username" and display only the filenames of the files that contain the search string.

Overall, the "sls" command is a useful tool for searching for specific strings or patterns in files and can be used to quickly locate data or information. However, the exact functionality of the command might depend on the context it is being used in. 

## tldr 
 
> This command is an alias of `Select-String`.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/select-string>.

- View documentation for the original command:

`tldr where-object`
