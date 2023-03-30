# powershell 
## chatgpt 
PowerShell is an interactive command-line shell and scripting language used to automate and manage Windows operating system tasks. It is built on the .NET framework and includes a powerful suite of built-in tools and commands for managing and automating Windows systems.

To launch PowerShell, you can simply type "powershell" into the Start menu search box or command prompt on a Windows system. This will open a new PowerShell console window where you can begin typing commands.

PowerShell commands (known as cmdlets) follow a Verb-Noun syntax, where the verb describes the action you want to perform and the noun specifies the object you want to perform the action on. For example, if you want to view the contents of a directory, you would type:

```powershell
Get-ChildItem C:\Users\YourUserName\Desktop
```

This command uses the "Get-ChildItem" cmdlet to retrieve a list of files and folders in the Desktop directory of the current user.

PowerShell also supports pipelining, which allows you to chain together multiple commands to perform complex tasks. For example, you could use the following command to find all TXT files on your desktop and sort them by file size:

```powershell
Get-ChildItem C:\Users\YourUserName\Desktop -Filter *.txt | Sort-Object Length
```

This command first retrieves all files on the Desktop directory that have a .txt extension using the "Get-ChildItem" cmdlet. It then pipes the resulting list of files to the "Sort-Object" cmdlet, which sorts the files by their length (in bytes).

Overall, PowerShell is a powerful tool for managing and automating Windows systems, and its extensive library of built-in cmdlets and support for third-party modules make it a versatile and flexible tool for IT professionals and power users. 

## tldr 
 
> Command-line shell and scripting language designed especially for system administration.
> See also: `pwsh`.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/powershell>.

- Start an interactive shell session:

`powershell`

- Start an interactive shell session without loading startup configs:

`powershell -NoProfile`

- Execute specific commands:

`powershell -Command "{{echo 'powershell is executed'}}"`

- Execute a specific script:

`powershell -File {{path/to/script.ps1}}`

- Start a session with a specific version of PowerShell:

`powershell -Version {{version}}`

- Prevent a shell from exit after running startup commands:

`powershell -NoExit`

- Describe the format of data sent to PowerShell:

`powershell -InputFormat {{Text|XML}}`

- Determine how an output from PowerShell is formatted:

`powershell -OutputFormat {{Text|XML}}`
