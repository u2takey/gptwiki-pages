# Tee-Object 
## chatgpt 
The `Tee-Object` command is a PowerShell cmdlet that is used to display console output and write it to a file at the same time. The tee command takes command output as input and outputs it both to the screen and to a file.

Syntax: 

```
command | Tee-Object [-FilePath] <string> [-Append] [-Delimiter <char>] [-Encoding <Encoding>] [-InputObject <psobject>]

```

Parameters:

- **-FilePath** (required): specifies the file path and name where you want to save the output. 
- **-Append**: it appends the output to an existing file instead of overwriting it.
- **-Delimiter**: specifies the character delimiter to separate items in the output file. 
- **-Encoding**: specifies the encoding type of the output file (ASCII, Unicode, UTF8, etc.). 
- **-InputObject**: specifies the input object that contains the data to be used as output.

For example, if you want to display network information and save it to a file named 'network-info.txt' in the C:\Temp directory, you would use the following command:

```
Get-NetAdapter | Tee-Object -FilePath 'C:\Temp\network-info.txt'
```

This will display the network adapter information on the console and also write it to the 'network-info.txt' file on the specified directory. 

## tldr 
 
> Saves command output in a file or variable and also sends it down the pipeline.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/tee-object>.

- Output processes to a file and to the console:

`Get-Process | Tee-Object -FilePath {{path\to\file}}`

- Output processes to a variable and `Select-Object`:

`Get-Process notepad | Tee-Object -Variable {{proc}} | Select-Object processname,handles`
