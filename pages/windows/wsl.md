# wsl 
## chatgpt 
The "wsl" command is used in Windows 10 to launch the Windows Subsystem for Linux (WSL) instance installed on the system. 

WSL allows users to run Linux command-line tools and applications directly on Windows without having to install a separate operating system. 

When you enter the "wsl" command in the command prompt or PowerShell, it will open a Linux shell prompt or terminal where you can enter Linux commands and execute Linux applications.

Once in the WSL, users can execute various Linux commands such as "ls" (list files), "cd" (change directory), "mkdir" (make directory), and many more. Users can also install and use Linux applications via package managers like apt or yum.

Overall, the "wsl" command provides Windows users with an easy way to work with Linux tools and applications on their Windows machines without having to set up a virtual machine or dual-boot the system. 

## tldr 
 
> Manage the Windows Subsystem for Linux from the command-line.
> More information: <https://learn.microsoft.com/windows/wsl/reference>.

- Start a Linux shell (in the default distribution):

`wsl {{shell_command}}`

- Run a Linux command without using a shell:

`wsl --exec {{command}} {{command_arguments}}`

- Specify a particular distribution:

`wsl --distribution {{distribution}} {{shell_command}}`

- List available distributions:

`wsl --list`

- Export a distribution to a `.tar` file:

`wsl --export {{distribution}} {{path\to\distro_file.tar}}`

- Import a distribution from a `.tar` file:

`wsl --import {{distribution}} {{path\to\install_location}} {{path/to/distro_file.tar}}`

- Change the version of wsl used for the specified distribution:

`wsl --set-version {{distribution}} {{version}}`

- Shut down Windows Subsystem for Linux:

`wsl --shutdown`
