# doas 
## chatgpt 
The "doas" command is a Unix-like operating system command that is used to execute a command or set of commands with administrator or root privileges. It is similar to the "sudo" command, but with a simpler configuration and less complexity.

The "doas" command allows certain users or groups to execute privileged commands, with specific permissions granted through a configuration file located at "/etc/doas.conf". The configuration file specifies the allowed commands, users, and hosts, and the level of privileges that are granted.

The syntax for using "doas" command is as follows:

```
doas [options] command [arguments]
```

Here, "options" are the flags or switches that modify the behavior of the command, and "command" is the executable command or script that needs to be run with elevated privileges.

Some of the commonly used options with the "doas" command include:

- "-c" - to run a command as another user or group.
- "-u" - to specify the username to run the command as.
- "-s" - to run the shell specified in the SHELL environment variable.

Overall, the "doas" command provides a secure and convenient way to run privileged commands on Unix-like systems while limiting access to specific users, commands, and hosts. 

## tldr 
 
> Executes a command as another user.
> More information: <https://man.openbsd.org/doas>.

- Run a command as root:

`doas {{command}}`

- Run a command as another user:

`doas -u {{user}} {{command}}`

- Launch the default shell as root:

`doas -s`

- Parse a config file and check if the execution of a command as another user is allowed:

`doas -C {{config_file}} {{command}}`

- Make `doas` request a password even after it was supplied earlier:

`doas -L`
