# smbclient 
## chatgpt 
Smbclient is a command-line tool that is used to connect to and interact with servers and shares that use the Server Message Block (SMB) protocol. The SMB protocol is a powerful network protocol that is used to share files, printers, and other resources between computers.

Smbclient command is used to connect to a remote SMB/CIFS server, and it allows the user to perform various operations on the remote server, such as listing directories, accessing files, and transferring data.

Here are some of the important options and flags that can be used with the smbclient command:

- -U: This option is used to specify the username that will be used to authenticate with the remote server.

- -N: This option is used to specify that the client should not send any authentication information, and instead, the server should assume that the client is anonymous.

- -L: This option is used to list the shares available on the remote server.

- -c: This option is used to specify a command that should be executed on the remote server after the client has connected.

- get: This command is used to copy a file from the remote server to the local machine.

- put: This command is used to copy a file from the local machine to the remote server.

- ls: This command is used to list the contents of a directory on the remote server.

Overall, smbclient is a powerful and flexible tool that can be used to interact with SMB/CIFS servers and shares from the command line. 

## tldr 
 
> FTP-like client to access SMB/CIFS resources on servers.
> More information: <https://manned.org/smbclient>.

- Connect to a share (user will be prompted for password; `exit` to quit the session):

`smbclient {{//server/share}}`

- Connect with a different username:

`smbclient {{//server/share}} --user {{username}}`

- Connect with a different workgroup:

`smbclient {{//server/share}} --workgroup {{domain}} --user {{username}}`

- Connect with a username and password:

`smbclient {{//server/share}} --user {{username%password}}`

- Download a file from the server:

`smbclient {{//server/share}} --directory {{path/to/directory}} --command "get {{file.txt}}"`

- Upload a file to the server:

`smbclient {{//server/share}} --directory {{path/to/directory}} --command "put {{file.txt}}"`

- List the shares from a server anonymously:

`smbclient --list={{server}} --no-pass`
