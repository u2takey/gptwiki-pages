# xprop 
## chatgpt 
The `xprop` command in Linux and other Unix-based systems is used to display the properties of X windows. It is particularly useful for debugging or analyzing a window system's behavior.

When the command is run, it opens an X window and waits for the user to click on a window. Once a window is selected, `xprop` will display a list of properties associated with the selected window. These properties include the window's ID, class, name, type, and more.

Users can also use `xprop` to set properties for a window by adding additional flags and arguments. For example, using the `-set` flag followed by the name of a property and its value will update that specific property for the selected window.

Overall, `xprop` is a powerful command-line utility that can help users gain insight into the workings of their window system and make changes as needed. 

## tldr 
 
> A tool for displaying window and font properties in an X server.
> More information: <https://manned.org/xprop>.

- Display the name of the root window:

`xprop -root WM_NAME`

- Display the window manager hints for a window:

`xprop -name "{{window_name}}" WM_HINTS`

- Display the point size of a font:

`xprop -font "{{font_name}}" POINT_SIZE`

- Display all the properties of the window with the id 0x200007:

`xprop -id {{0x200007}}`
