# qjoypad 
## chatgpt 
QJoyPad is a Linux-based graphical user interface application that allows users to map any keyboard or joystick action to any other joystick button, keyboard key, or mouse button. It provides a simple interface for mapping various types of input devices to other devices, allowing users to play games and run applications more efficiently.

To use QJoyPad, open the application and start mapping the input devices to other devices. Users can choose the type of input device to map, the device to map it to, and the action to perform when the mapped device is triggered.

For example, a user could map the X button on a joystick to the Escape key on the keyboard, allowing them to quickly exit an application or game.

Overall, QJoyPad is a useful tool for Linux users who want to improve their gaming or application experience by customizing their input devices. 

## tldr 
 
> Translate input from gamepads or joysticks into keyboard strokes or mouse actions.
> More information: <http://qjoypad.sourceforge.net/>.

- Start QJoyPad:

`qjoypad`

- Start QJoyPad and look for devices in a specific directory:

`qjoypad --device={{path/to/directory}}`

- Start QJoyPad but don't show a system tray icon:

`qjoypad --notray`

- Start QJoyPad and force the window manager to use a system tray icon:

`qjoypad --force-tray`

- Force a running instance of QJoyPad to update its list of devices and layouts:

`qjoypad --update`

- Load the given layout in an already running instance of QJoyPad, or start QJoyPad using the given layout:

`qjoypad "{{layout}}"`
