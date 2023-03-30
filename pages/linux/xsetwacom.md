# xsetwacom 
## chatgpt 
xsetwacom is a command-line tool used to configure Wacom tablet devices on Linux systems. It allows the user to set various properties of the tablet, such as the sensitivity of the stylus, the pressure curve, and the mapping between the tablet and the screen.

The command xsetwacom is typically followed by a number of subcommands and options that specify the desired changes to the tablet’s configuration. For example, the command xsetwacom set "Device Name" PressureCurve 0 40 60 80 will change the pressure curve of the device named "Device Name" to 0 at 0% pressure, 40 at 25% pressure, 60 at 50% pressure, and 80 at 75% pressure.

Other common subcommands include set, get, and list. The set subcommand allows the user to set a specific property value, the get subcommand allows the user to retrieve the current value of a property, and the list subcommand shows a list of available properties for a device.

Overall, xsetwacom is a powerful tool for customizing the configuration of Wacom tablet devices on Linux systems, and can help users to optimize their tablet settings and achieve a better workflow. 

## tldr 
 
> Command-line tool to change settings for Wacom pen tablets at runtime.
> More information: <https://manned.org/xsetwacom>.

- List all the available Wacom devices. The device name is in the first column:

`xsetwacom list`

- Set Wacom area to specific screen. Get name of the screen with `xrandr`:

`xsetwacom set "{{device_name}}" MapToOutput {{screen}}`

- Set mode to relative (like a mouse) or absolute (like a pen) mode:

`xsetwacom set "{{device_name}}" Mode "{{Relative|Absolute}}"`

- Rotate the input (useful for tablet-PC when rotating screen) by 0|90|180|270 degrees from "natural" rotation:

`xsetwacom set "{{device_name}}" Rotate {{none|half|cw|ccw}}`

- Set button to only work when the tip of the pen is touching the tablet:

`xsetwacom set "{{device_name}}" TabletPCButton "on"`
