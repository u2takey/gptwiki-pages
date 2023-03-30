# ftp 
## chatgpt 
FTP (File Transfer Protocol) is a standard Internet protocol used to transfer files between computers on a network. It is a client-server protocol, which means that one computer (the client) sends a request to another computer (the server) for a file, and the server responds by sending the file over the network.

The "ftp" command is a command line tool used to initiate an FTP session with a remote server. It allows users to transfer files to and from remote servers that are running an FTP server, and also allows users to perform other FTP operations like creating, modifying, and deleting files and directories on the remote server.

To use the ftp command, you need to know the hostname or IP address of the remote server, as well as a valid username and password for the server. Once you have this information, you can open a command prompt or terminal window, and enter the following command:

```
ftp <server_address>
```

Where "<server_address>" is the hostname or IP address of the remote server. After entering this command, you'll be prompted to enter your username and password for the server. Once you've successfully authenticated, you'll be able to enter other FTP commands to perform various operations on the remote server.

Common FTP commands include:

- get <remote_file>: Downloads the specified file from the remote server to your local computer.
- put <local_file>: Uploads the specified file from your local computer to the remote server.
- ls: Lists the files and directories in the current directory on the remote server.
- cd <directory>: Changes the current directory on the remote server.
- mkdir <directory>: Creates a new directory on the remote server.
- rmdir <directory>: Deletes a directory on the remote server.
- delete <remote_file>: Deletes the specified file from the remote server.

Once you're finished using FTP, you can use the "quit" command to end your session and disconnect from the remote server. 

## tldr 
 
> Tools to interact with a server via File Transfer Protocol.
> More information: <https://manned.org/ftp>.

- Connect to an FTP server:

`ftp {{ftp.example.com}}`

- Connect to an FTP server specifying its IP address and port:

`ftp {{ip_address}} {{port}}`

- Switch to binary transfer mode (graphics, compressed files, etc):

`binary`

- Transfer multiple files without prompting for confirmation on every file:

`prompt off`

- Download multiple files (glob expression):

`mget {{*.png}}`

- Upload multiple files (glob expression):

`mput {{*.zip}}`

- Delete multiple files on the remote server:

`mdelete {{*.txt}}`

- Rename a file on the remote server:

`rename {{original_filename}} {{new_filename}}`
