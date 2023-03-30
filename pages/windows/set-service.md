# Set-Service 
## chatgpt 
The Set-Service command in PowerShell is used to modify the properties of an existing Windows Service. It allows you to change the state of the service, modify its startup type and dependencies, update the service description, and other related properties.

Here is the basic syntax for the Set-Service command:

```powershell
Set-Service [-Name] <String> [[-DisplayName] <String>] [[-Status] <ServiceControllerStatus>] [[-StartupType] <ServiceStartMode>] [[-Description] <String>] [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```
- `Name`: The name of the service you want to modify.
- `DisplayName`: The display name of the service that you want to modify.
- `Status`: The new status of the service you want to set (Running, Stopped, Paused, etc).
- `StartupType`: The new startup type of the service (Automatic, Manual, Disabled, etc).
- `Description`: The new description of the service that you want to set.
- `PassThru`: This parameter is used to return the updated service object back to the pipeline. 
- `WhatIf`: This parameter simulates the service changes to confirm whether you want the changes to actually take effect.
- `Confirm`: This parameter prompts you for confirmation before proceeding with the changes.

For example, to set the startup type of a service called "MyService" to automatic, run the following command:

```powershell
Set-Service -Name MyService -StartupType Automatic
```

This will set the startup type of the MyService to Automatic. Similarly, you can modify other properties of the service using the Set-Service command. 

## tldr 
 
> Starts, stops, and suspends a service, and changes its properties.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.management/set-service>.

- Change a display name:

`Set-Service -Name {{hostname}} -DisplayName "{{name}}"`

- Change the startup type of services:

`Set-Service -Name {{service_name}} -StartupType {{Automatic}}`

- Change the description of a service:

`Set-Service -Name {{service_name}} -Description "{{description}}"`
