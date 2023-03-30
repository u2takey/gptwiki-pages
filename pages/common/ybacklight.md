# ybacklight 
## chatgpt 
As an AI language model, I don't have knowledge of all commands as it depends on the operating system where you are using this command. However, based on my general knowledge, "ybacklight" is not a standard command that is found in most operating systems. In most cases, the command used to adjust backlight on a computer screen is "xbacklight" which is used for X server.

The "xbacklight" command accesses the backlight brightness controls located in the file system and adjusts the brightness based on the arguments passed. The command syntax for xbacklight is as follows:

`xbacklight [+-][percentage]`

Where "+-" indicates increase or decrease in brightness and "percentage" is the number of units by which you want to increase or decrease the brightness. 

For example, if you want to decrease the display brightness by 30%, you would type:

`xbacklight -30`

This command will be particularly useful when you are running some program or a script in a dark environment and you want to decrease the screen brightness to avoid eye strain or disturbance. 

## tldr 
 
> Manage screen backlight brightness. See also `xbacklight`.
> More information: <https://github.com/pixelcmtd/ybacklight>.

- Print current brightness and maximal brightness, shortened and separated by a slash:

`ybacklight Sc/Sm`

- Set the brightness to 420:

`ybacklight s{{420}}`

- Increase the brightness by 42 big steps (4200 by default):

`ybacklight Si{{42}}`

- Decrease the brightness by 300:

`ybacklight d{{300}}`
