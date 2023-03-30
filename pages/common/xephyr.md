# Xephyr 
## chatgpt 
Xephyr is a command used to start a nested X server that runs inside a regular X window system session. It is a tool for running a virtual X server inside an existing X server. It creates a new, smaller, window that can contain another X server session.

The syntax of the Xephyr command is:

```
Xephyr [options] :displaynumber [options]
```

Some of the commonly used options are:

- -screen: specifies the screen size for the nested X server.
- -resizeable: allows the nested X server to be resized.
- -fullscreen: starts the nested X server in full-screen mode.
- -dpi: specifies the dots per inch for the nested X server.
- -query host: allows connections from another machine to the nested X server.

The displaynumber argument specifies the X display number that the nested X server will listen on. It must be unique and not already in use by another X server.

Once the Xephyr command is executed, a new window will open that contains the nested X server. You can then run applications and window managers inside this window, just as you would with a regular X server.

Xephyr is particularly useful for testing and debugging purposes as it allows you to run multiple X environments on a single machine without needing additional hardware. 

## tldr 
 
> A nested X server that runs as an X application.
> More information: <https://manned.org/xserver-xephyr>.

- Create a black window with display ID ":2":

`Xephyr -br -ac -noreset -screen {{800x600}} {{:2}}`

- Start an X application on the new screen:

`DISPLAY=:2 {{command_name}}`
