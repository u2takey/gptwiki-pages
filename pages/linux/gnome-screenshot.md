# gnome-screenshot 
## chatgpt 
The `gnome-screenshot` command is a Linux command-line tool that allows users to take a screenshot of their desktop or a specific window. When the command is executed in a terminal, it captures an image of either the entire screen or a specific window, depending on the parameters used with the command.

Here are some of the parameters that can be used with the `gnome-screenshot` command:

- `-a` or `--area`: allows the user to define a specific rectangular area of the screen to be captured.
- `-w` or `--window`: captures the active window.
- `-d` or `--delay`: adds a delay of a specified number of seconds before taking the screenshot.
- `-f` or `--file`: defines a filename and directory where the screenshot will be saved.

When executed without any parameters, the `gnome-screenshot` command takes a screenshot of the entire screen and saves it to the user's home directory. The resulting image file is usually named something like `Screenshot from [date timestamp].png`.

Overall, the `gnome-screenshot` command is a simple but useful tool for taking screenshots on Linux-based operating systems. 

## tldr 
 
> Capture the screen, a window, or a user-defined area and save the image to a file.
> More information: <https://manned.org/gnome-screenshot>.

- Take a screenshot and save it to the default location, normally `~/Pictures`:

`gnome-screenshot`

- Take a screenshot and save it to the named file location:

`gnome-screenshot --file {{path/to/file}}`

- Take a screenshot and save it to the clipboard:

`gnome-screenshot --clipboard`

- Take a screenshot after the specified number of seconds:

`gnome-screenshot --delay {{5}}`

- Launch the GNOME Screenshot GUI:

`gnome-screenshot --interactive`

- Take a screenshot of the current window and save it to the specified file location:

`gnome-screenshot --window --file {{path/to/file}}`

- Take a screenshot after the specified number of seconds and save it to the clipboard:

`gnome-screenshot --delay {{10}} --clipboard`

- Display the version:

`gnome-screenshot --version`
