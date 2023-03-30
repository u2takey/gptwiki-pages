# vncserver 
## chatgpt 
The `vncserver` command is used to start a VNC (Virtual Network Computing) server on a Linux system. 

VNC is a graphical desktop sharing system that allows users to remotely access and control another computer or virtual machine over a network connection. 

When "vncserver" is executed, it performs the following steps:

1. Starts a new VNC server session on the specified display number (e.g. ":1").
2. Generates a unique desktop session ID for the new VNC server session.
3. Creates a new desktop environment on the server, using the specified window manager (or defaults to the desktop environment's default window manager if none is specified).
4. Starts a VNC client listener process on the specified port number, allowing remote clients to connect to and control the VNC server session.

The VNC server session will continue running until it is stopped using the `vncserver -kill` command or the system is restarted. 

By default, the VNC server requires a password to connect, which can be set using the `vncpasswd` command. 

Overall, the `vncserver` command is a useful tool for remote administration and access to Linux systems. 

## tldr 
 
> Launches a VNC (Virtual Network Computing) desktop.
> More information: <https://manned.org/vncserver.1x>.

- Launch a VNC Server on next available display:

`vncserver`

- Launch a VNC Server with specific screen geometry:

`vncserver --geometry {{width}}x{{height}}`

- Kill an instance of VNC Server running on a specific display:

`vncserver --kill :{{display_number}}`
