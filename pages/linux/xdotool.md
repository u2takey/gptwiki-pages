# xdotool 
## chatgpt 
`xdotool` is a command-line tool for simulating user input and manipulating windows in X Window System. It allows you to automate repetitive tasks or implement custom keyboard shortcuts.

Here are some examples of how to use `xdotool`:

1. Simulating key presses:

To simulate a key press, use the following syntax:

```
xdotool key [keycode/keysym]
```

For example, to simulate pressing the "a" key:

```
xdotool key a
```

Or to simulate pressing the "Enter" key:

```
xdotool key Return
```

2. Moving and resizing windows:

To move a window, use the following syntax:

```
xdotool windowmove [window_id] [x] [y]
```

For example, to move the current window to the top left corner:

```
xdotool getactivewindow windowmove 0 0
```

To resize a window, use the following syntax:

```
xdotool windowsize [window_id] [width] [height]
```

For example, to resize the current window to 800x600:

```
xdotool getactivewindow windowsize 800 600
```

3. Clicking and dragging:

To simulate a mouse click, use the following syntax:

```
xdotool click [button]
```

For example, to simulate a left click:

```
xdotool click 1
```

To simulate a mouse drag, use the following syntax:

```
xdotool mousedown [button] && xdotool mousemove [x] [y] && xdotool mouseup [button]
```

For example, to drag a file from one folder to another:

```
xdotool mousedown 1 && xdotool mousemove 100 100 && xdotool mouseup 1
```

Note that you need to replace `[button]`, `[x]` and `[y]` with the desired values in the above examples.

This is just a small sample of what `xdotool` can do. It's a powerful tool that can be used in many different ways to automate tasks and improve productivity on the Linux desktop. 

## tldr 
 
> Command-line automation for X11.
> More information: <https://manned.org/xdotool>.

- Retrieve the X-Windows window ID of the running Firefox window(s):

`xdotool search --onlyvisible --name {{firefox}}`

- Click the right mouse button:

`xdotool click {{3}}`

- Get the ID of the currently active window:

`xdotool getactivewindow`

- Focus on the window with ID of 12345:

`xdotool windowfocus --sync {{12345}}`

- Type a message, with a 500ms delay for each letter:

`xdotool type --delay {{500}} "Hello world"`

- Press the enter key:

`xdotool key {{KP_Enter}}`
