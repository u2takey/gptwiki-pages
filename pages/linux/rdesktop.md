# rdesktop 
## chatgpt 
rdesktop is a command-line tool used to connect to a remote Windows desktop environment. It allows a user to access and control a Windows desktop from a Linux or Unix-based system.

The basic syntax for the rdesktop command is:

rdesktop [options] [server]

Options are additional parameters that can be used with the command to customize the connection parameters. Some of the most commonly used options include:

- -u: specify the username for the remote desktop connection
- -p: specify the password for the remote desktop connection
- -a: use the specified color depth (in bits) for the remote desktop session
- -g: set the desktop size for the remote session (in pixels)
- -k: specify the keyboard layout for the remote desktop session
- -s: specify a shell to run on the remote server

The server parameter specifies the name or IP address of the remote Windows desktop to connect to. Once a connection is established, the user can interact with the remote desktop as if they were physically sitting in front of it.

Overall, the rdesktop command is a powerful tool that enables remote access to Windows desktops from Linux or Unix-based systems. It is commonly used in enterprise settings where users need to access Windows-based applications from non-Windows environments. 

## tldr 
 
> Remote Desktop Protocol client.
> It can be used to connect the remote computer using the RDP protocol.
> More information: <https://manned.org/rdesktop>.

- Connect to a remote computer (default port is 3389):

`rdesktop -u {{username}} -p {{password}} {{host:port}}`

- Simple Examples:

`rdesktop -u Administrator -p passwd123 192.168.1.111:3389`

- Connect to a remote computer with full screen (press `Ctrl + Alt + Enter` to exist):

`rdesktop -u {{username}} -p {{password}} -f {{host:port}}`

- Use the customed resolution (use the letter 'x' between the number):

`rdesktop -u {{username}} -p {{password}} -g 1366x768 {{host:port}}`

- Connect to a remote computer using domain user:

`rdesktop -u {{username}} -p {{password}} -d {{domainname}} {{host:port}}`

- Use the 16-bit color (speed up):

`rdesktop -u {{username}} -p {{password}} -a 16 {{host:port}}`
