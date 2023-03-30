# wmic 
## chatgpt 
The "wmic" command is short for "Windows Management Instrumentation Command-line," which is a utility included in most versions of the Windows operating system. It allows users to interact with Windows Management Instrumentation (WMI) and perform administrative tasks from the command line.

WMI is an interface that provides access to management information and operational data about a system, such as hardware components, software applications, processes, services, and networking configurations. WMI can be used to monitor system performance, troubleshoot issues, and manage resources remotely.

The "wmic" command can be used to query and manipulate WMI data from the command line. It accepts a variety of parameters and options that allow users to retrieve information about system properties and components, run system commands, and configure various settings.

Some examples of "wmic" commands include:

- "wmic cpu get name": Retrieves the name of the processor installed on the system.
- "wmic process get name, processid": Lists the names and process IDs of all running processes.
- "wmic service where "state='stopped'" get name": Displays the names of all stopped services on the system.
- "wmic useraccount where "name='%USERNAME%'" get sid": Returns the security identifier (SID) of the current user.

Overall, the "wmic" command is a powerful and flexible tool for managing and troubleshooting Windows systems from the command line. 

## tldr 
 
> Interactive shell for detailed information about running processes.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/wmic>.

- Fundamental grammar:

`wmic {{alias}} {{where_clause}} {{verb_clause}}`

- Show brief details about the currently running processes:

`wmic process list brief`

- Show full details about the currently running processes:

`wmic process list full`

- Access specific fields such as process name, process ID and parent process ID:

`wmic process get {{name,processid,parentprocessid}}`

- Display information about a specific process:

`wmic process where {{name="example.exe"}} list full`

- Display specific fields for a specific process:

`wmic process where processid={{pid}} get {{name,commandline}}`

- Kill a process:

`wmic process {{pid}} delete`
