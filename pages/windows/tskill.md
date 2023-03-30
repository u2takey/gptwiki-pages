# tskill 
## chatgpt 
The `tskill` command is a Windows command used to end a specific task or process by its process ID or by its name. It is a short form of "Taskkill". 

Syntax: `tskill [Process ID | Process Name]`

Process ID: It identifies the process that needs to be terminated. To find a process ID, open the task manager and go to the Process tab. The PID column shows the process ID.

Process Name: It identifies the name of the process that needs to be terminated. The process name should be exact and case-sensitive.

For example, to terminate a process with process ID `1234`, the command would be:

`tskill 1234`

And to terminate a process named "chrome.exe", the command would be:

`tskill chrome.exe`

When the command is executed, it forcefully terminates the respective process, and all the unsaved data or work in the process is lost. It is suggested to save your work before using this command. 

## tldr 
 
> Ends a process running in a session on a Remote Desktop Session Host.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/tskill>.

- Terminate a process by its process identifier:

`tskill {{process_id}}`

- Terminate a process by its name:

`tskill {{process_name}}`
