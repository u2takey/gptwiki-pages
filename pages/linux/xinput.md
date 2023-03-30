# xinput 
## chatgpt 
The xinput command is a tool for configuring input devices in the X Window System on Linux and other Unix-like operating systems. It allows users to manipulate and customize input devices such as keyboards, mice, trackpads, joysticks, and touchscreens.

When executed with no arguments, the xinput command displays a list of all input devices connected to the system, along with their names, IDs, and other attributes such as whether the device is enabled, what relative or absolute dimensions it reports, or if it has any pointer or keyboard emulation settings.

Some of the most commonly used options for the xinput command include:

- --list-props <device>: Displays a list of properties that can be configured for the specified device, including the current value of each property.
- --set-prop <device> <property> <value>: Sets the value of the specified property for the specified device.
- --get-button-map <device>: Displays the current button mapping for the specified device, which determines how the physical buttons on the device are mapped to virtual buttons in the X input system. 
- --set-button-map <device> <map>: Changes the button map for the specified device to the values passed in <map>, where each number represents the virtual button that the corresponding physical button should be mapped to.

Overall, xinput is a powerful and flexible command-line utility that allows users to configure and customize their input devices to suit their needs and preferences. 

## tldr 
 
> List available input devices, query information about a device and change input device settings.
> More information: <https://manned.org/xinput>.

- List all input devices:

`xinput list`

- Disable an input:

`xinput disable {{id}}`

- Enable an input:

`xinput enable {{id}}`

- Disconnect an input from its master:

`xinput float {{id}}`

- Reattach an input as slave to a master:

`xinput reattach {{id}} {{master_id}}`

- List settings of an input device:

`xinput list-props {{id}}`

- Change a setting of an input device:

`xinput set-prop {{id}} {{setting_id}} {{value}}`
