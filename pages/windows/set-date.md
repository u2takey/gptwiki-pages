# Set-Date 
## chatgpt 
The Set-Date command is a PowerShell cmdlet that allows users to set the system date and time on a computer. When executed, the command changes the date and time settings to the specified values.

Syntax:
Set-Date [-date] <DateTime> [-computername <String>] [-force] [-whatif] [-confirm] [<CommonParameters>]

Parameters:
-Date: The new system date and time to be set. The parameter accepts an input in the form of a DateTime object.

-Computername: Specifies the name of the computer whose system date and time need to be set. If not specified, the command sets the system date and time on the local computer.

-Force: Forces the command to execute without any prompts or warnings.

-WhatIf: Displays a preview of the changes that will happen when the command is executed.

-Confirm: Prompts the user to confirm the command before executing.

Examples:
To set the system date and time to August 22, 2021 at 9:35 pm, use the following command:
Set-Date "8/22/2021 9:35 PM"

To set the system date and time on a remote computer named "Server1", use the following command:
Set-Date -Date "8/22/2021 9:35 PM" -ComputerName Server1

Note: The Set-Date command requires administrative privileges to execute. It should be used with caution as incorrect settings could cause issues with system functionality. 

## tldr 
 
> Changes the system time on the computer to a time that you specify.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/set-date>.

- Add three days to the system date:

`Set-Date -Date (Get-Date).AddDays({{3}})`

- Set the system clock back 10 minutes:

`Set-Date -Adjust -0:10:0 -DisplayHint Time`

- Add 90 minutes to the system clock:

`$90mins = New-TimeSpan -Minutes {{90}}; Set-Date -Adjust $90mins`
