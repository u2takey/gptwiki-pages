# transfersh 
## chatgpt 
transfersh is a command line tool used for transferring files between two systems. It is used to share files quickly and easily without having to go through complicated file-sharing processes.

The transfersh command works by creating a temporary link that is valid for 24 hours. The file can be downloaded using this link by anyone who has access to it. The command line tool uses HTTPS for secure file transfer.

The transfersh command is very easy to use. To share a file, simply type "transfersh [FILE NAME]" on the command line. The tool will upload the file and provide a URL that can be shared with others. To download a file, simply follow the provided URL and save the file to your computer.

The advantage of using transfersh is that it simplifies file sharing by creating temporary links that can be shared easily. It also provides a level of security by using HTTPS for file transfer. Additionally, the tool does not require the installation of any software or registration, making it a convenient option for users who want to share files quickly on-the-go. 

## tldr 
 
> An unofficial command-line client for transfer.sh.
> More information: <https://github.com/AlpixTM/transfersh>.

- Upload a file to transfer.sh:

`transfersh {{path/to/file}}`

- Upload a file showing a progress bar (requires Python package `requests_toolbelt`):

`transfersh --progress {{path/to/file}}`

- Upload a file using a different file name:

`transfersh --name {{filename}} {{path/to/file}}`

- Upload a file to a custom transfer.sh server:

`transfersh --servername {{upload.server.name}} {{path/to/file}}`

- Upload all files from a directory recursively:

`transfersh --recursive {{path/to/directory/}}`

- Upload a specific directory as an uncompressed tar:

`transfersh -rt {{path/to/directory}}`
