# Wait-Process 
## chatgpt 
The "Wait-Process" command is a PowerShell cmdlet that waits for a specified process or processes to complete before proceeding with the next step in a script or command sequence. 

To use the "Wait-Process" command, you need to specify the name or process ID of the process or processes that the command should wait for. For example, if you want to wait for a process with the name "MyProcess.exe" to complete, you would use the following command:

```
Wait-Process -Name "MyProcess.exe"
```

Alternatively, if you know the process ID of the process you want to wait for, you can use the following command:

```
Wait-Process -Id 1234
```

In both cases, the command will block the execution until the specified process has completed or terminated. If the process completes successfully, the command returns with no output. However, if the process terminates with an error or is unable to complete, an error message will be displayed in the console.

The "Wait-Process" command is often used in automation or scripting scenarios where multiple processes need to be run in a specific order or sequence, ensuring that each process completes before the next one starts. It is also useful when you need to pause a script until a specific process has completed before proceeding further. 

## tldr 
 
> Waits for the processes to be stopped before accepting more input.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.management/wait-process>.

- Stop a process and wait:

`Stop-Process -Id {{process_id}}; Wait-Process -Id {{process_id}}`

- Wait for processes for a specified time:

`Wait-Process -Name {{process_name}} -Timeout {{30}}`
