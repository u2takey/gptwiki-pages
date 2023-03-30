# fondue 
## chatgpt 
Fondue is a command used in Linux and Unix operating systems to manage File Transfer Protocol (FTP) files. The command allows users to interact with FTP servers and transfer files to and from them. 

The basic structure of the command is as follows:

fondue [options] [username[:password]@]hostname[:port]/[remote-dir]/[filename] [local-file]

Here's what each part of the command means:

- [options]: This is an optional parameter that you can use to modify the behavior of the command. For example, you might use the -v option to enable verbose output, or the -P option to specify the FTP data port.

- [username[:password]@]: This part of the command specifies the credentials you want to use to log in to the FTP server. You can include a username, a password (if required), and an "@" character to separate them from the hostname part of the command.

- hostname[:port]: This specifies the hostname or IP address of the FTP server you want to connect to. You can also specify a port number using the ":" character.

- /[remote-dir]/[filename]: This part of the command specifies the remote directory and file you want to transfer. You can include a full path, or just the name of the folder and the file.

- [local-file]: This is the local file you want to transfer, and can be a fully qualified local file path or just the file name. 

Once you have entered the command correctly, you can use it to transfer files to and from the FTP server, use it to delete files on the server, or manage directory listings. 

It is essential to ensure that the FTP server you are attempting to transfer files from is legitimate, and you have the correct credentials to access your desired files, and in cases where you are uploading personal data, it is recommended to use encrypted FTP or SFTP to protect your data. 

## tldr 
 
> A command-line installer for optional Windows features.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/fondue>.

- Enable a specific Windows feature:

`fondue /enable-feature:{{feature}}`

- Hide all output messages to the user:

`fondue /enable-feature:{{feature}} /hide-ux:all`

- Specify a caller process name for error reporting:

`fondue /enable-feature:{{feature}} /caller-name:{{name}}`
