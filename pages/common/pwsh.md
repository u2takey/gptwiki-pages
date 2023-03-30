# pwsh 
## chatgpt 
The command "pwsh" is used to launch PowerShell on a machine. PowerShell is a command-line shell and scripting language that is designed to help IT professionals automate and manage various tasks in Windows systems, including server administration, network management, and security management.

When the pwsh command is executed, it initiates the PowerShell environment, providing access to its command-line interface and functionality. The pwsh command launches PowerShell Core, which is an open-source version of PowerShell that is designed to work on various platforms, such as Windows, Linux, and macOS.

PowerShell Core provides various features and capabilities, including advanced scripting capabilities, cross-platform support, efficient execution of batch operations, easy integration with existing IT tools and processes, and more. With PowerShell, IT professionals can create and execute complex scripts to automate various tasks, including system management, application deployment, data processing, and more. 

## tldr 
 
> PowerShell Core is a cross-platform automation and configuration tool/framework.
> See also: `powershell`.
> More information: <https://learn.microsoft.com/powershell/>.

- Start an interactive shell session:

`pwsh`

- Start an interactive shell session without loading startup configs:

`pwsh -NoProfile`

- Execute specific commands:

`pwsh -Command "{{string}}"`

- Execute a specific script:

`pwsh {{path/to/script.ps1}}`

- Start an interactive shell session with a specific execution policy:

`pwsh -ExecutionPolicy {{AllSigned|Bypass|Default|RemoteSigned|Restricted|...}}`
