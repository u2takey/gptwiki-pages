# msiexec 
## chatgpt 
Msiexec (short for Microsoft Windows Installer Executable) is a command-line tool used by Microsoft Windows operating system to install, modify, and uninstall software programs that use Microsoft Installer (MSI) technology. It is used by software developers and system administrators to automate the process of software installation and maintenance. The command is used to execute Windows Installer package (.msi files), some sample usage of the command are as follows:

1. Install an MSI package: msiexec /i "path-to-msi-file"

2. Uninstall an MSI package: msiexec /x "path-to-msi-file"

3. Repair an MSI package: msiexec /f "path-to-msi-file"

4. Update an MSI package: msiexec /p "path-to-msi-file"

5. Install silently: msiexec /i "path-to-msi-file" /qn

The command also allows for a range of options, including logging, verbose output, administrative installation, patching, and customization. Msiexec can also be used in conjunction with Group Policy to deploy software across multiple machines in a network. It is a powerful tool for managing software installations and simplifying the process of software deployment and management. 

## tldr 
 
> Install, update, repair, or uninstall Windows programs using MSI and MSP package files.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/msiexec>.

- Install a program from its MSI package:

`msiexec /package {{path\to\file.msi}}`

- Install a MSI package from a website:

`msiexec /package {{https://example.com/installer.msi}}`

- Install a MSP patch file:

`msiexec /update {{path\to\file.msp}}`

- Uninstall a program or patch using their respective MSI or MSP file:

`msiexec /uninstall {{path\to\file}}`
