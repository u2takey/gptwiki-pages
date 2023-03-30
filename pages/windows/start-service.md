# Start-Service 
## chatgpt 
Start-Service is a PowerShell cmdlet used to start a Windows service running on a local or remote computer. Services are programs that run in the background and provide functionality to other programs or users, such as printing, networking, or security services.

The syntax for the Start-Service cmdlet is as follows:
Start-Service [-Name]<String[]> [[-Exclude] <String[]>] [-PassThru] [-Verbose] [-WhatIf] [-Confirm] [<CommonParameters>]

-Name: This parameter specifies the name of the Windows service that you want to start. You can provide multiple service names separated by commas.

-Exclude: This optional parameter specifies one or more service names that you want to exclude from the operation.

-PassThru: This optional parameter returns the service object representing the service that was started. You can use the returned object for further processing.

-Verbose: This optional parameter displays detailed information during the operation.

-WhatIf: This optional parameter displays what would happen if the cmdlet is run, without actually performing the operation.

-Confirm: This optional parameter prompts the user to confirm the operation before it is performed.

Example:
Start-Service -Name "Print Spooler" -Verbose
This command starts the Print Spooler service and displays verbose output during the operation. 

## tldr 
 
> Starts one or more stopped services.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.management/start-service>.

- Start a service by using its name:

`Start-Service -Name {{service_name}}`

- Display information without starting a service:

`Start-Service -DisplayName *{{name}}* -WhatIf`

- Start a disabled service:

`Set-Service {{service_name}} -StartupType {{manual}}; Start-Service {{service_name}}`
