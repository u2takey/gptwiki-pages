# lftp 
## chatgpt 
lftp is a command-line file transfer program which allows users to transfer files between local and remote systems. It is similar to other FTP clients like FileZilla or WinSCP, but is used via the command line rather than a graphical user interface (GUI).

The basic syntax for using lftp is:

lftp [options] [site]

where options are various command-line switches that modify the behavior of lftp, and site is the address of the remote system you wish to connect to (e.g., ftp.example.com).

Once connected to the remote system, lftp allows you to perform a variety of operations. These include:

- Uploading and downloading files: You can transfer files between your local system and the remote system using the get and put commands.

- Managing directories: The cd and lcd commands allow you to navigate between directories on the remote system and your local system, respectively. The mkdir and rmdir commands allow you to create and delete directories on the remote system.

- Managing files: The rm command can be used to delete files on the remote system, while the mv and cp commands allow you to move and copy files, respectively.

- Other operations: Lftp also supports a variety of other commands, such as chmod for changing file permissions, du for displaying disk usage, and more.

Overall, lftp is a powerful command-line tool for file transfers that offers a wide range of features and functionality. However, it may require some experience with the command line to use effectively. 

## tldr 
 
> Sophisticated file transfer program.
> More information: <https://lftp.yar.ru/lftp-man.html>.

- Connect to an FTP server:

`lftp --user {{username}} {{ftp.example.com}}`

- Download multiple files (glob expression):

`mget {{path/to/*.png}}`

- Upload multiple files (glob expression):

`mput {{path/to/*.zip}}`

- Delete multiple files on the remote server:

`mrm {{path/to/*.txt}}`

- Rename a file on the remote server:

`mv {{original_filename}} {{new_filename}}`

- Download or update an entire directory:

`mirror {{path/to/remote_dir}} {{path/to/local_output_dir}}`

- Upload or update an entire directory:

`mirror -R {{path/to/local_dir}} {{path/to/remote_output_dir}}`
