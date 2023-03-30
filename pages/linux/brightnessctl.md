# brightnessctl 
## chatgpt 
brightnessctl is a command-line utility that is used to control the screen brightness of a display. It allows users to adjust the brightness level of the display on their Linux operating system easily.

The brightnessctl command is used by specifying a parameter or an option with the command, followed by the brightness level to which the display brightness is to be set. The brightness levels are represented as a percentage or as a value that ranges from 0 to 100 depending on the display.

Here are some examples of the brightnessctl command:

1. To get the current brightness level of the display, run the command without any parameters or options:
```
brightnessctl
```

2. To set the brightness level to a specific value, run the following command, where the percentage value should be replaced with the desired brightness level:
```
brightnessctl set <percentage>
```

3. To increase or decrease the current brightness level of the display, run the following command. The change in brightness level should be replaced with a positive or negative value, respectively:
```
brightnessctl set <change>%+
brightnessctl set <change>%-
```

4. To turn off or on the display, run the following commands:
```
brightnessctl set 0
brightnessctl set max
```

Overall, the brightnessctl command is used to adjust the display brightness effectively and quickly on a Linux system. 

## tldr 
 
> Utility for reading and controlling device brightness for GNU/Linux operating systems.
> More information: <https://github.com/Hummer12007/brightnessctl>.

- List devices with changeable brightness:

`brightnessctl --list`

- Print the current brightness of the display backlight:

`brightnessctl get`

- Set the brightness of the display backlight to a specified percentage within range:

`brightnessctl set {{50%}}`

- Increase brightness by a specified increment:

`brightnessctl set {{+10%}}`

- Decrease brightness by a specified decrement:

`brightnessctl set {{10%-}}`
