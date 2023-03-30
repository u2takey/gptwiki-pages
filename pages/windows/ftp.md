# ftp 
## chatgpt 
FTP stands for File Transfer Protocol. It is a standard network protocol used for transferring files from one host to another over the internet. The FTP command is a command-line utility that is used to connect to an FTP server and perform various file transfer operations.

The basic syntax of the FTP command is as follows:

```
ftp [options] hostname
```

Here, "options" specifies the various command-line options that can be used with the FTP command. "hostname" specifies the hostname or IP address of the remote FTP server that you want to connect to.

Once you run the FTP command, it will prompt you to enter your login credentials (username and password) for the FTP server. Once you are logged in, you can use various commands to perform file transfer operations like uploading, downloading, deleting, renaming, and creating directories.

Some of the common FTP commands are:

- ls: List the contents of the current directory.
- cd: Change the current directory.
- get: Download a file from the server.
- put: Upload a file to the server.
- mget: Download multiple files.
- mput: Upload multiple files.
- mkdir: Create a new directory.
- rmdir: Remove a directory.
- delete: Delete a file.

Overall, the FTP command is a powerful tool for transferring files over the internet in a secure and efficient manner. It is widely used by businesses, developers, and individuals for various file transfer operations. 

## tldr 
 
> Interactively transfer files between a local and remote FTP server.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/ftp>.

- Connect to a remote FTP server interactively:

`ftp {{host}}`

- Log in as an anonymous user:

`ftp -A {{host}}`

- Disable automatic login upon initial connection:

`ftp -n {{host}}`

- Run a file containing a list of FTP commands:

`ftp -s:{{path\to\file}} {{host}}`

- Download multiple files (glob expression):

`mget {{*.png}}`

- Upload multiple files (glob expression):

`mput {{*.zip}}`

- Delete multiple files on the remote server:

`mdelete {{*.txt}}`

- Display detailed help:

`ftp --help`
