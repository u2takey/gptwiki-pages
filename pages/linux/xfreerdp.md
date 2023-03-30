# xfreerdp 
## chatgpt 
The `xfreerdp` command is a software utility used to remotely connect to a Windows Terminal Server or Remote Desktop Server. It is an open-source implementation of the Remote Desktop Protocol (RDP) client.

The command requires specific arguments to function, including the IP address or hostname of the Windows server to connect to, the username and password to use for authentication, and various other configuration settings.

The syntax of the `xfreerdp` command is as follows:

```
xfreerdp [options] server[:port] [/v:server[:port]] [/u:user] [/p:password] [session] 
```

Here are some of the important options you can use with the `xfreerdp` command:

- `-u`: Specifies the username for authentication purposes.
- `-p`: Specifies the password for authentication purposes.
- `/v`: Specifies the hostname or IP address of the Windows server to connect to.
- `/size`: Specifies the screen resolution to use for the remote desktop session.
- `/f`: Launches the remote desktop session in fullscreen mode.
- `/audio-mode`: Specifies the audio output mode to use for the remote desktop session.
- `/cert-ignore`: Ignores SSL certificate errors that may occur during the connection.

There are many other options you can use with the `xfreerdp` command, and you can find a full list of them in the command's documentation. 

## tldr 
 
> Free Remote Desktop Protocol implementation.
> More information: <https://www.freerdp.com>.

- Connect to a FreeRDP server:

`xfreerdp /u:{{username}} /p:{{password}} /v:{{ip_address}}`

- Connect to a FreeRDP server and activate audio output redirection using `sys:alsa` device:

`xfreerdp /u:{{username}} /p:{{password}} /v:{{ip_address}} /sound:{{sys:alsa}}`

- Connect to a FreeRDP server with dynamic resolution:

`xfreerdp /v:{{ip_address}} /u:{{username}} /p:{{password}} /dynamic-resolution`

- Connect to a FreeRDP server with clipboard redirection:

`xfreerdp /v:{{ip_address}} /u:{{username}} /p:{{password}} +clipboard`

- Connect to a FreeRDP server ignoring any certificate checks:

`xfreerdp /v:{{ip_address}} /u:{{username}} /p:{{password}} /cert:ignore`
