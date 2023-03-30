# rpcclient 
## chatgpt 
The `rpcclient` command is a tool used in Linux and Unix systems to perform Remote Procedure Call (RPC) operations on a Windows system. It is often used for administrative tasks on a Windows domain, such as managing users, groups, shares, and permissions.

RPC is a communication protocol that allows a program to request services from another program located on a different computer or server across a network. With `rpcclient`, a user can remotely access Windows servers and manage some of the services available on these servers.

The syntax for the `rpcclient` command is as follows:

```
rpcclient [-U username] [-W domain] [-c command] [-d debug_level] [-k] [-N] [-P password] [-p port] [-R realm] [-s service] destination
```

Here, `destination` is the IP address or hostname of the Windows server that you want to access.

Other options include:

- `-U username`: Specifies the username to connect to the remote server. If not provided, the current user will be used.
- `-W domain`: Specifies the domain name to which the user belongs.
- `-c command`: Executes the specified command on the remote server.
- `-d debug_level`: Sets the debug level for the output.
- `-k`: Uses Kerberos authentication instead of NTLM authentication.
- `-N`: Tells `rpcclient` to use null authentication.
- `-P password`: Specifies the password for the user.
- `-p port`: Specifies the port number to use for the RPC connections.
- `-R realm`: Specifies the realm for the user.
- `-s service`: Specifies the service name to connect to on the remote server.

Once connected to the Windows server using `rpcclient`, a user can execute commands to manage the server. These commands are similar to those used on Windows command line tools like `net user`, `net group`, `net share`, and `icacls`.

Overall, `rpcclient` is a powerful tool for remotely managing Windows servers and can be very useful for system administrators tasked with managing a large number of Windows machines. 

## tldr 
 
> MS-RPC client tool (part of the samba suite).
> More information: <https://www.samba.org/samba/docs/current/man-html/rpcclient.1.html>.

- Connect to a remote host:

`rpcclient --user {{domain}}\{{username}}%{{password}} {{ip}}`

- Connect to a remote host on a domain without a password:

`rpcclient --user {{username}} --workgroup {{domain}} --no-pass {{ip}}`

- Connect to a remote host, passing the password hash:

`rpcclient --user {{domain}}\{{username}} --pw-nt-hash {{ip}}`

- Execute shell commands on a remote host:

`rpcclient --user {{domain}}\{{username}}%{{password}} --command {{semicolon_separated_commands}} {{ip}}`

- Display domain users:

`rpcclient $> enumdomusers`

- Display privileges:

`rpcclient $> enumprivs`

- Display information about a specific user:

`rpcclient $> queryuser {{username|rid}}`

- Create a new user in the domain:

`rpcclient $> createdomuser {{username}}`
