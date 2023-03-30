# x11vnc 
## chatgpt 
The 'x11vnc' command is used to start and control a Virtual Network Computing (VNC) server on an X window system. This allows remote access to a graphical desktop environment running on a UNIX-like operating system through a VNC viewer. 

Some of the key options that can be used with the 'x11vnc' command include:

- -auth: Specifies the X authority file to use for authentication with the X server. 
- -display: Specifies the display to use. By default, it uses the value specified in the DISPLAY environment variable. 
- -passwd: Specifies the password file to use for authentication. 
- -rfbauth: Specifies the file containing the VNC password to use for authentication. 
- -forever: Causes the server to keep running even if the client disconnects. 
- -shared: Allows multiple clients to connect to the VNC server simultaneously. 
- -noxdamage: Disables the 'xdamage' extension, which can cause issues with some VNC viewers. 

The 'x11vnc' command can be used in a variety of scenarios, such as remote support, remote administration, or accessing a machine without a dedicated monitor or keyboard. 

## tldr 
 
> A VNC server that will enable VNC on an existing display server.
> By default, the server will automatically terminate once all clients disconnect from it.
> More information: <https://manned.org/x11vnc>.

- Launch a VNC server that allows multiple clients to connect:

`x11vnc -shared`

- Launch a VNC server in view-only mode, and which won't terminate once the last client disconnects:

`x11vnc -forever -viewonly`

- Launch a VNC server on a specific display and screen (both starting at index zero):

`x11vnc -display :{{display}}.{{screen}}`

- Launch a VNC server on the third display's default screen:

`x11vnc -display :{{2}}`

- Launch a VNC server on the first display's second screen:

`x11vnc -display :{{0}}.{{1}}`
