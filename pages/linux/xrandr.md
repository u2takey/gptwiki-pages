# xrandr 
## chatgpt 
The `xrandr` command is a Linux-based command-line tool used to configure and manage display settings for an X Window System. Some of the functions of the `xrandr` command include:

1. Displaying the available display devices that are connected to the computer.
2. Modifying display settings, such as the resolution and refresh rate of the monitor.
3. Rotating the screen orientation.
4. Mirroring or extending the display to multiple monitors.
5. Configuring the primary monitor.

The `xrandr` command is typically used by system administrators and power users who require fine-grained control over the display settings. When executed, the `xrandr` command will show a list of connected display devices, along with their resolutions and display settings. The user can then modify the settings using additional command-line options.

For example, `xrandr` can be used to set the resolution of a monitor as follows:

```
xrandr --output HDMI-1 --mode 1920x1080
```

In this example, `HDMI-1` is the name of the monitor, and `--mode 1920x1080` sets the resolution to 1920x1080.

Overall, the `xrandr` command gives users greater control over their display settings and is a useful tool in managing multiple displays. 

## tldr 
 
> Set the size, orientation and/or reflection of the outputs for a screen.
> More information: <https://www.x.org/releases/current/doc/man/man1/xrandr.1.xhtml>.

- Display the current state of the system (known screens, resolutions, ...):

`xrandr --query`

- Disable disconnected outputs and enable connected ones with default settings:

`xrandr --auto`

- Change the resolution and update frequency of DisplayPort 1 to 1920x1080, 60Hz:

`xrandr --output {{DP1}} --mode {{1920x1080}} --rate {{60}}`

- Set the resolution of HDMI2 to 1280x1024 and put it on the right of DP1:

`xrandr --output {{HDMI2}} --mode {{1280x1024}} --right-of {{DP1}}`

- Disable the VGA1 output:

`xrandr --output {{VGA1}} --off`

- Set the brightness for LVDS1 to 50%:

`xrandr --output {{LVDS1}} --brightness {{0.5}}`
