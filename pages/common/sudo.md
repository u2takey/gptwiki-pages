# sudo 
## chatgpt 
sudo stands for "superuser do" and is a command used in Unix/Linux operating systems that allows a user to run commands with elevated privileges or as the "superuser" or "root user". 

It is typically used when a regular user account does not have enough permissions to execute a command, and the command requires elevated access rights to run. 

The sudo command works by temporarily elevating the user's privileges, allowing them to run the command with full root privileges. The user is prompted to enter their password before executing the command, to ensure that they have appropriate permissions to run the command.

The syntax for using the sudo command is: 

```
sudo [options] [command]
```

Where [options] are any additional flags or options you want to pass to the command, and [command] is the command you want to run with elevated privileges.

Examples of using the sudo command include installing system updates, modifying system files, and managing user accounts. 

## tldr 
 
> Executes a single command as the superuser or another user.
> More information: <https://www.sudo.ws/sudo.html>.

- Run a command as the superuser:

`sudo {{less /var/log/syslog}}`

- Edit a file as the superuser with your default editor:

`sudo --edit {{/etc/fstab}}`

- Run a command as another user and/or group:

`sudo --user={{user}} --group={{group}} {{id -a}}`

- Repeat the last command prefixed with `sudo` (only in `bash`, `zsh`, etc.):

`sudo !!`

- Launch the default shell with superuser privileges and run login-specific files (`.profile`, `.bash_profile`, etc.):

`sudo --login`

- Launch the default shell with superuser privileges without changing the environment:

`sudo --shell`

- Launch the default shell as the specified user, loading the user's environment and reading login-specific files (`.profile`, `.bash_profile`, etc.):

`sudo --login --user={{user}}`

- List the allowed (and forbidden) commands for the invoking user:

`sudo --list`
