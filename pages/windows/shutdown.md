# shutdown 
## chatgpt 
The command "shutdown" is a system command used in computer operating systems to halt or power off the system. This command is used when a user wants to shut down the computer or a system administrator wants to remotely shut down a networked computer. 

This command provides several options for the user to customize the way the shutdown process happens. These options include:

1. -s: This option is used when the user wants to shut down the computer completely.

2. -r: This option is used when the user wants to restart the computer.

3. -h: This option is used to hibernate the computer.

4. -t xx: This option is used to set the time in seconds after which the shutdown process will begin.

5. -f: This option is used to force the programs to close, without giving the user an option to save their work.

6. -m \\computername: This option is used to remotely shut down a networked computer.

In summary, the shutdown command is a powerful yet simple tool used to shut down or restart a computer or remotely shut down a networked computer with customizable options. 

## tldr 
 
> A tool for shutting down, restarting or logging off a machine.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/shutdown>.

- Shutdown the current machine:

`shutdown /s`

- Shutdown the current machine force-closing all apps:

`shutdown /s /f`

- Restart the current machine immediately:

`shutdown /r /t 0`

- Hibernate the current machine:

`shutdown /h`

- Log off the current machine:

`shutdown /l`

- Specify a timeout in seconds to wait before shutting down:

`shutdown /s /t {{8}}`

- Abort a shutdown sequence whose timeout is yet to expire:

`shutdown /a`

- Shutdown a remote machine:

`shutdown /m {{\\hostname}}`
