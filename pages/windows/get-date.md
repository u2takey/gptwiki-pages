# Get-Date 
## chatgpt 
The Get-Date command is a PowerShell cmdlet that retrieves the current date and time of the system where the command is executed. It returns an object of the System.DateTime type that contains information about the date, time, and time zone.

Syntax:
Get-Date [[-Date] <DateTime>] [[-DisplayHint] {Date | Time | DateTime | DayOfWeek}] [-Format <String>] [-UFormat <String>] [<CommonParameters>]

Parameters:
-Date: The DateTime object to retrieve the date and time value.
-DisplayHint: Specifies how to display the date and time value. It can be either 'Date', 'Time', 'DateTime', or 'DayOfWeek'.
-Format: Specifies the custom format to display the date and time value.
-UFormat: Specifies the Unix format to display the date and time value.
-CommonParameters: Includes parameters that can be used with any PowerShell cmdlets.

Examples:
- Get-Date: Retrieves the current date and time of the system.
- Get-Date -DisplayHint Time: Retrieves the current time of the system.
- Get-Date -Format "MM/dd/yyyy": Retrieves the current date of the system in the format of month/day/year.
- Get-Date -UFormat %s: Retrieves the Unix timestamp of the current date and time. 

## tldr 
 
> Gets the current date and time.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/get-date>.

- Display the current date and time:

`Get-Date`

- Display the current date and time with a .NET format specifier:

`Get-Date -Format "{{yyyy-MM-dd HH:mm:ss}}"`

- Display the current date and time in UTC and ISO 8601 format:

`(Get-Date).ToUniversalTime()`

- Convert a Unix timestamp:

`Get-Date -UnixTimeSeconds {{1577836800}}`
