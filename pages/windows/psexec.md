# psexec 
## chatgpt 
Psexec is a command-line tool that allows system administrators to remotely execute processes on other systems, particularly those running Windows operating systems. It is a part of the PsTools suite provided by Microsoft.

The syntax of the command is:

```
psexec \\computer -u username -p password command
```

Here, `\\computer` specifies the name of the remote computer where the command should be executed. `-u username` and `-p password` specify the credentials of a user account on the remote computer with sufficient privileges to execute the command. `command` specifies the command to be executed on the remote computer.

Psexec provides a range of options to fine-tune the behavior of the tool, such as running the command under a different user account, specifying a different port for communication, or redirecting output to a file.

Overall, psexec enables administrators to automate tasks and deploy software remotely, making it a valuable tool for managing networks and distributed systems. 

## tldr 
 
> Execute a command-line process on a remote machine.
> This is an advanced command and it might potentially be dangerous.
> More information: <https://learn.microsoft.com/en-us/sysinternals/downloads/psexec>.

- Execute a command using `cmd` in a remote shell:

`psexec \\{{remote_host}} cmd`

- Execute a command on a remote host (pre-authenticated):

`psexec \\{{remote_host}} -u {{user_name}} -p {{password}}`

- Execute a command remotely and output the result to a file:

`psexec \\{{remote_host}} cmd /c {{command}} -an ^>{{path\to\file.txt}}`

- Execute a program to interact with users:

`psexec \\{{remote_host}} -d -i {{program_name}}`

- Display the IP configuration of the remote host:

`psexec \\{{remote_host}} ipconfig /all`
