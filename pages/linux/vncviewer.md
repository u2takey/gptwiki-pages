# vncviewer 
## chatgpt 
The vncviewer command is a command-line utility that allows an individual to view a remote desktop that is running on a VNC (Virtual Network Computing) server. The basic syntax of the command is:

```
vncviewer [options] hostname[:display#]
```

- `[options]`: This refers to any additional arguments that can be supplied with the command to modify its behavior, such as the display size or authentication options.
- `hostname`: This refers to the name or IP address of the remote server that the individual wishes to connect to.
- `display#`: This refers to the display number of the remote server that the individual wishes to access.

The vncviewer command establishes a connection to the VNC server running on the remote host and displays the contents of the remote desktop on the individual's local desktop. This allows the individual to interact with the remote desktop as if they were sitting in front of it. The VNC server must be installed and running on the remote host. Additionally, the individual must have the necessary permissions to access the remote server. 

## tldr 
 
> Launches a VNC (Virtual Network Computing) client.
> More information: <https://manned.org/vncviewer>.

- Launch a VNC client which connects to a host on a given display:

`vncviewer {{host}}:{{display_number}}`

- Launch in full-screen mode:

`vncviewer -FullScreen {{host}}:{{display_number}}`

- Launch a VNC client with a specific screen geometry:

`vncviewer --geometry {{width}}x{{height}} {{host}}:{{display_number}}`

- Launch a VNC client which connects to a host on a given port:

`vncviewer {{host}}::{{port}}`
