# xbacklight 
## chatgpt 
The `xbacklight` command is a utility program used to adjust the backlight brightness of a display with an X server (the program that manages graphical interfaces in Linux/Unix systems). 

When executed, the `xbacklight` command reads and sets the brightness level of the display. It is often used in conjunction with keyboard shortcuts or scripts to modify backlight levels.

The syntax for the command is as follows:

```
xbacklight [-help] [-set <percentage>] [-time <milliseconds>] [-get] [-inc <percentage>] [-dec <percentage>]
```

The options available for this command are:

- `-help` prints a help message about the usage of the xbacklight command.
- `-set` sets the backlight brightness to a specific percentage value. For example, `-set 50` sets the brightness to 50%.
- `-time` sets the time (in milliseconds) needed to perform the brightness transition from one level to the other. For example, `-time 200` sets the transition time to 200 ms.
- `-get` displays the current brightness level of the display. For example, `-get` returns the current brightness percentage.
- `-inc` increases the brightness level by a set percentage value. For example, `-inc 10` increases the brightness by 10%.
- `-dec` decreases the brightness level by a set percentage value. For example, `-dec 10` decreases the brightness by 10%.

Note that the xbacklight command may not work on all systems, particularly if the hardware does not implement brightness controls to the operating system. 

## tldr 
 
> Utility to adjust backlight brightness using the RandR extension.
> More information: <https://gitlab.freedesktop.org/xorg/app/xbacklight>.

- Get the current screen brightness as a percentage:

`xbacklight`

- Set the screen brightness to 40%:

`xbacklight -set {{40}}`

- Increase current brightness by 25%:

`xbacklight -inc {{25}}`

- Decrease current brightness by 75%:

`xbacklight -dec {{75}}`

- Increase backlight to 100%, over 60 seconds (value given in ms), using 60 steps:

`xbacklight -set {{100}} -time {{60000}} -steps {{60}}`
