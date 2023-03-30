# Out-String 
## chatgpt 
The Out-String command is a Windows PowerShell cmdlet that takes the input object or objects and converts them to a string. This command is mostly used to display the output of a command as a single string, which makes it easier to view and manipulate the output.

The Out-String cmdlet can be used in various ways. Here are a few examples:

1. You can pipe the output of a command to Out-String and specify the width of the screen. This command will wrap the text to fit the screen.

Example command: 

Get-Help Out-String | Out-String -Width 80

This command will display the help content of the Out-String cmdlet as a string, wrapping the text to fit the screen width of 80.

2. You can use Out-String to join the output of multiple commands into a single string.

Example command:

(Get-Process | Select-Object -First 10 | Format-Table | Out-String) + "`r`n" + (Get-Service | Select-Object -First 10 | Format-Table | Out-String)

This command fetches the top 10 process and services and formats the output as a table. Then, the output of both commands is concatenated using + and stored as a string.

3. You can also use Out-String to display the output of a script as a string.

Example command:

./myscript.ps1 | Out-String

This command runs the script "myscript.ps1" and displays the output as a string using the Out-String cmdlet.

In summary, the Out-String command in Windows PowerShell converts the input object or objects into a string format that can be used to manipulate or display the output of a command as a single string. 

## tldr 
 
> Outputs input objects as a string.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/out-string>.

- Print host information as string:

`Get-Alias | Out-String`

- Convert each object to a string rather than concatenating all the objects into a single string:

`Get-Alias | Out-String -Stream`

- Use the `Width` parameter to prevent truncation:

`@{TestKey = ('x' * 200)} | Out-String -Width {{250}}`
