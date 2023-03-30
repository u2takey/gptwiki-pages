# unclutter 
## chatgpt 
The "unclutter" command is a Linux command that is used to hide the mouse cursor from the screen when there is no activity for a certain amount of time. This is useful when giving presentations or when watching a video because it reduces the visual distractions on the screen.

The command works by monitoring the mouse cursor and hiding it after a specified time of inactivity. By default, the cursor will appear again when the mouse is moved or when a key is pressed on the keyboard.

The syntax for using the "unclutter" command is:

unclutter [options]

Some of the common options for the "unclutter" command are:

- -display DISPLAY: Specifies the X display to use.
- -idle SECONDS: Sets the time in seconds of inactivity before hiding the cursor. The default is 5 seconds.
- -jitter PIXELS: Sets the maximum distance in pixels the cursor can move before being considered active. The default is 10 pixels.
- -key: Specifies that the cursor should reappear when a key is pressed instead of a mouse movement.

For example, to run the "unclutter" command with a 10 second idle time and a maximum jitter of 20 pixels, the command would be:

unclutter -idle 10 -jitter 20 

## tldr 
 
> Hides the mouse cursor.
> More information: <https://manned.org/unclutter.1x>.

- Hide mouse cursor after 3 seconds:

`unclutter -idle {{3}}`
