# whoami 
## chatgpt 
The "whoami" command is a Unix-based command that is used to display the current user name or login name of the user who is currently logged into the system. It is usually used in command-line interfaces like the Terminal in macOS and Command Prompt in Windows.

When executed, the "whoami" command outputs the current username of the user who initiated the command. This can be useful in shell scripts or command-line tools where you need to get the current user's name programmatically.

Here's an example of what the "whoami" command output might look like:

```
$ whoami
john
```

In this case, the output shows that the current user's username is "john". 

## tldr 
 
> Display details about the current user.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/whoami>.

- Display the username of the current user:

`whoami`

- Display the groups that the current user is a member of:

`whoami /groups`

- Display the privileges of the current user:

`whoami /priv`

- Display the user principal name (UPN) of the current user:

`whoami /upn`

- Display the logon ID of the current user:

`whoami /logonid`

- Display all information for the current user:

`whoami /all`
