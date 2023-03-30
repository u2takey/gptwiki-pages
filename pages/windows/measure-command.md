# Measure-Command 
## chatgpt 
The Measure-Command command in PowerShell is used to measure the amount of time taken by a PowerShell command or script block to process or execute. 

This command calculates the duration of the operation by determining the difference between the start time and end time of the operation. The duration is measured in seconds, milliseconds, or ticks. 

To use the Measure-Command command, you need to provide the command or script block you want to measure as an argument, enclosed in quotes or curly brackets. For example:

```
Measure-Command {Get-ChildItem C:\Windows}
```

This command will measure the amount of time taken to execute the Get-ChildItem command on the C:\Windows directory, and output the duration in the default format.

The Measure-Command command can also be used to measure the time taken by a script block or a pipeline of commands, by enclosing them in curly braces. For example:

```
Measure-Command {Get-ChildItem C:\Windows | Where-Object {$_.Length -gt 1MB} | Sort-Object Length}
```

This command will measure the time taken to execute the pipeline of three commands, and output the duration in the default format.

In addition to the default output, the Measure-Command command provides several parameters that you can use to customize the output, such as -Expression, -AsMilliseconds, -AsTicks, and -OutVariable. These parameters allow you to store the result in a variable, specify the time unit for the duration, and more. 

Overall, the Measure-Command command is a useful tool for measuring and benchmarking the performance of PowerShell commands and scripts. 

## tldr 
 
> Measures the time it takes to run script blocks and cmdlets.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/measure-command>.

- Measure the time it takes to run a command:

`Measure-Command { {{command}} }`

- Pipe input to Measure-Command (objects that are piped to `Measure-Command` are available to the script block that is passed to the Expression parameter):

`10, 20, 50 | Measure-Command -Expression { for ($i=0; $i -lt $_; $i++) {$i} }`
