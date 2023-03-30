# smbget 
## chatgpt 
Smbget is a command line utility tool used to download files from SMB/CIFS servers. The SMB/CIFS protocol is used for sharing files, printers, and other resources between networked computers. The smbget command is similar to the FTP and HTTP utilities, and it allows users to download files securely from SMB/CIFS servers.

Here is the syntax for using smbget command:

smbget [OPTIONS] smb://username:password@server/share/filename

Where,
- [OPTIONS] specifies the options for the smbget command.
- smb:// specifies the protocol to use for downloading the file.
- username is the name of the user account that has access to the shared folder.
- password is the password for the user account.
- server is the name or IP address of the SMB/CIFS server.
- share is the name of the shared folder.
- filename is the name of the file that you want to download from the shared folder.

Some common options available with smbget command are:
- -u username: specifies the username for authentication.
- -p password: specifies the password for authentication.
- -a: specifies anonymous authentication.
- -r: Specifies recursive download of directories.

For example, to download a file named "example.txt" from a shared folder "data" on the server "192.168.1.10" using the username "john" and password "12345", you can use the following command:

smbget -u john -p 12345 smb://192.168.1.10/data/example.txt

This will download the file "example.txt" from the share directory "data" on the server "192.168.1.10" into the current working directory of the local machine. 

## tldr 
 
> `wget`-like utility for downloading files from SMB servers.
> More information: <https://www.samba.org/samba/docs/current/man-html/smbget.1.html>.

- Download a file from a server:

`smbget {{smb://server/share/file}}`

- Download a share or directory recursively:

`smbget --recursive {{smb://server/share}}`

- Connect with a username and password:

`smbget {{smb://server/share/file}} --user {{username%password}}`

- Require encrypted transfers:

`smbget {{smb://server/share/file}} --encrypt`
