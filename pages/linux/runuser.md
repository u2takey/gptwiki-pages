# runuser 
## chatgpt 
The `runuser` command is used in Linux and Unix-based operating systems to run a command or a shell as a different user identity. This command is used to temporarily switch the privileges to the specified user, execute the command or shell, and then return to the original identity of the active user.

The syntax of the `runuser` command is as follows:

```
runuser [OPTION]... [-u USER] COMMAND
```

Here, the options can be used to set environment variables, specify the home directory, or define the user ID or group ID. `-u USER` option is used to specify the user whose privileges need to be switched. `COMMAND` is the command or shell that needs to be run as that user.

For example, to run the command `ls` as user Alice, the command can be written as:

```
runuser -u alice ls
```

Here, the `runuser` command temporarily switches to the user account `alice` and runs the `ls` command. Once the command is executed, the command shell returns to its original user identity.

In summary, the `runuser` command is used to run a command or shell as a different user, and it is especially useful when running administrative tasks that require higher privileges than the current user has. 

## tldr 
 
> Run commands as a specific user and group without asking for password (needs root privileges).
> More information: <https://manned.org/runuser>.

- Run command as a different user:

`runuser {{user}} -c '{{command}}'`

- Run command as a different user and group:

`runuser {{user}} -g {{group}} -c '{{command}}'`

- Start a login shell as a specific user:

`runuser {{user}} -l`

- Specify a shell for running instead of the default shell (also works for login):

`runuser {{user}} -s {{/bin/sh}}`

- Preserve the entire environment of root (only if `--login` is not specified):

`runuser {{user}} --preserve-environment -c '{{command}}'`
