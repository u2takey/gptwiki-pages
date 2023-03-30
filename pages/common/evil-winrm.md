# evil-winrm 
## chatgpt 
Evil-winrm is a command-line tool used for remote code execution and lateral movement in Windows environments. It is a tool modeled after the popular Linux tool, "psexec". 

The command "evil-winrm" is used to connect to a remote Windows server or workstation over the network using Windows Remote Management (WinRM) protocol. This command is executed to establish a remote shell session on the target machine, enabling users to run PowerShell commands remotely for various tasks such as running scripts, performing recon, and executing commands.

The syntax of the command is as follows:

`evil-winrm -i <target-ip> -u <username> [-p <password> | -H <hash>]`

Where:

- `-i` specifies the IP address or hostname of the target machine.
- `-u` specifies the username to authenticate with on the target machine.
- `-p` is the optional plaintext password to authenticate with.
- `-H` is the optional password hash to authenticate with.

Once authenticated, you will be presented with a remote PowerShell prompt on the target machine that you can use to execute various commands and interact with the remote system. Evil-winrm is a powerful tool and, as the name suggests, it can be used for both legitimate and malicious purposes. So, it should be used with caution and only in authorized situations. 

## tldr 
 
> Windows Remote Management (WinRM) shell for pentesting.
> Once connected, we get a PowerShell prompt on the target host.
> More information: <https://github.com/Hackplayers/evil-winrm>.

- Connect to a host:

`evil-winrm --ip {{ip}} --user {{user}} --password {{password}}`

- Connect to a host, passing the password hash:

`evil-winrm --ip {{ip}} --user {{user}} --hash {{nt_hash}}`

- Connect to a host, specifying directories for scripts and executables:

`evil-winrm --ip {{ip}} --user {{user}} --password {{password}} --scripts {{path/to/scripts}} --executables {{path/to/executables}}`

- Connect to a host, using SSL:

`evil-winrm --ip {{ip}} --user {{user}} --password {{password}} --ssl --pub-key {{path/to/pubkey}} --priv-key {{path/to/privkey}}`

- Upload a file to the host:

`PS > upload {{path/to/local/file}} {{path/to/remote/file}}`

- Get a list of loaded PowerShell functions:

`PS > menu`

- Load a PowerShell script from the `--scripts` directory:

`PS > {{script.ps1}}`

- Invoke a binary on the host from the `--executables` directory:

`PS > Invoke-Binary {{binary.exe}}`
