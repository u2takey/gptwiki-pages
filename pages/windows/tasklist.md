# tasklist 
## chatgpt 
The "tasklist" command is a Windows command-line utility that displays a list of all currently running processes on a computer, along with various details about each process. 

When the "tasklist" command is executed, it provides a table with the following information for each process: 

- Image Name: The name of the executable file for the process. 
- PID: The unique process identifier assigned to each process by the operating system. 
- Session Name: The name of the session in which the process is running. 
- Session# : The unique identifier for the session in which the process is running. 
- Mem Usage: The total amount of memory being used by the process (in kilobytes). 
- Status: Displays whether the process is "running," "not responding," or "unknown." 
- User Name: The name of the user account under which the process is running. 
- CPU Time: The amount of CPU time used by the process since it started. 
- Window Title: The title of the window that the process is associated with (if applicable). 

The "tasklist" command can be useful for troubleshooting performance issues, identifying resource intensive processes, and terminating unresponsive or malicious processes. It can also be used in batch files or scripts to automate process monitoring and managing. 

## tldr 
 
> Display a list of currently running processes on a local or remote machine.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/tasklist>.

- Display currently running processes:

`tasklist`

- Display running processes in a specified output format:

`tasklist /fo {{table|list|csv}}`

- Display running processes using the specified `.exe` or `.dll` file name:

`tasklist /m {{module_pattern}}`

- Display processes running on a remote machine:

`tasklist /s {{remote_name}} /u {{username}} /p {{password}}`

- Display services using each process:

`tasklist /svc`
