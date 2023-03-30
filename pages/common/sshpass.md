# sshpass 
## chatgpt 
`sshpass` is a command-line tool used to provide password to an SSH command without requiring interaction from the user. It allows users to automate ssh authentication by providing the password in the command-line itself. 

The `sshpass` command is used with the `ssh` command to provide the authentication password. The syntax for the command is as follows:

```
sshpass -p <password> ssh <user>@<host>
```

- `-p`: Option to provide password in the command line
- `<password>`: Authentication password for the SSH command
- `<user>`: Username to login with
- `<host>`: Hostname or IP address of the server to connect to

By using `sshpass`, users can skip the manual entry of the password, thereby enabling automation of the SSH authentication process. However, it is important to note that using `sshpass` with passwords in plain text could pose a security risk. It is recommended to use other SSH authentication methods, such as public key authentication, whenever possible. 

## tldr 
 
> An ssh password provider.
> It works by creating a TTY, feeding the password into it, and then redirecting `stdin` to the ssh session.
> More information: <https://manned.org/sshpass>.

- Connect to a remote server using a password supplied on a file descriptor (in this case, `stdin`):

`sshpass -d {{0}} ssh {{user}}@{{hostname}}`

- Connect to a remote server with the password supplied as an option, and automatically accept unknown ssh keys:

`sshpass -p {{password}} ssh -o StrictHostKeyChecking=no {{user}}@{{hostname}}`

- Connect to a remote server using the first line of a file as the password, automatically accept unknown ssh keys, and launch a command:

`sshpass -f {{path/to/file}} ssh -o StrictHostKeyChecking=no {{user}}@{{hostname}} "{{command}}"`
