# Select-String 
## chatgpt 
The Select-String command is used in PowerShell to search for specific strings or patterns within a file or a string variable. It can search for patterns in plain text files or in the output of PowerShell cmdlets, scripts, or functions.

The basic syntax of the Select-String command is:

```powershell
Select-String [-Pattern] <string[]> [-Path] <string[]> [-InputObject] <psobject[]> [-AllMatches] [-CaseSensitive] [-Context] <int[]>
```

Here is what each parameter means:

- `-Pattern`: Specifies one or more patterns to search for. The pattern can be a regular expression, wildcard character (* or ?), or a simple string.
- `-Path`: Specifies the file path(s) to search. It can be a single file or a list of files.
- `-InputObject`: Specifies the string variable or pipeline input to search within.
- `-AllMatches`: Specifies if the command should return all matches in a file or just the first match.
- `-CaseSensitive`: Specifies if the search is case sensitive or not.
- `-Context`: Specifies the number of lines before and after a match to include in the output.

Once the command is run, it will return an object with the properties of the matching line, the file name, and the line number. The output can also be piped to other cmdlets for further filtering or manipulation.

Here is an example of how to use the Select-String command to search for a specific pattern in a file:

```powershell
Select-String -Pattern "error" -Path "C:\Logs\mylog.txt"
```

This command will search for the word "error" in the file "C:\Logs\mylog.txt" and return all the lines that contain that word. 

## tldr 
 
> Finds text in strings and files in PowerShell.
> This command can only be used through PowerShell.
> You can use `Select-String` similar to grep in UNIX or findstr.exe in Windows.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/select-string>.

- Search for a pattern within a file:

`Select-String -Path "{{path\to\file}}" -Pattern '{{search_pattern}}'`

- Search for an exact string (disables regular expressions):

`Select-String -SimpleMatch "{{exact_string}}" {{path\to\file}}`

- Search for pattern in all `.ext` files in current dir:

`Select-String -Path "{{*.ext}}" -Pattern '{{search_pattern}}'`

- Capture the specified number of lines before and after the line that matches the pattern:

`Select-String --Context {{2,3}} "{{search_pattern}}" {{path\to\file}}`

- Search stdin for lines that do not match a pattern:

`Get-Content {{path\to\file}} | Select-String --NotMatch "{{search_pattern}}"`
