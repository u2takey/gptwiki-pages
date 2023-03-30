# uvcdynctrl 
## chatgpt 
uvcdynctrl is a command-line tool for dynamically controlling and configuring various settings of USB video devices that are compatible with the Video4Linux2 (V4L2) API. It allows you to interact with the device's controls and change settings such as brightness, contrast, hue, saturation, autofocus, exposure, white balance, and many more.

The basic syntax of the uvcdynctrl command is as follows:

```
uvcdynctrl [option] [control] [command]
```

Here, the 'option' is used to specify various command-line options, such as -h to display the help menu or -l to list all available controls for the connected device.

The 'control' argument refers to the name of the control that you want to modify. For example, 'Brightness', 'Contrast', 'Focus', etc.

The 'command' argument is used to change the value of the specified control. It can be a single integer value, or a string of values separated by colons indicating a range or a list of values. For example, to set the brightness level of a device to 50%, you would use the following command:

```
uvcdynctrl -s 'Brightness' 50
```

Some other commonly used commands and options with the uvcdynctrl tool are:

- -L: lists all available video devices
- -C: lists all available controls for the specified device
- -c: displays the current value of the specified control
- -S: saves the current settings of the device to a configuration file
- -R: restores the settings from a previously saved configuration file 

Overall, the uvcdynctrl command is a powerful tool for controlling the settings of USB video devices and can help you fine-tune the output of your webcam or other similar devices. 

## tldr 
 
> A libwebcam command-line tool to manage dynamic controls in uvcvideo.
> More information: <https://manned.org/uvcdynctrl>.

- List all available cameras:

`uvcdynctrl -l`

- Specify the device to use (defaults to `video0`):

`uvcdynctrl -d {{device_name}}`

- List available controls:

`uvcdynctrl -c`

- Set a new control value (for negative values, add -- before {{-value}}):

`uvcdynctrl -s {{control_name}} {{value}}`

- Get the current control value:

`uvcdynctrl -g {{control_name}}`

- Save the state of the current controls to a file:

`uvcdynctrl -W {{filename}}`

- Load the state of the controls from a file:

`uvcdynctrl -L {{filename}}`
