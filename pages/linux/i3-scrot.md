# i3-scrot 
## chatgpt 
The i3-scrot command is used to take screenshots on the i3 window manager. 

Here is a breakdown of the command:

- "i3" refers to the window manager, i3.
- "scrot" is short for "screen shot".
- Together, "i3-scrot" means to take a screenshot on the i3 window manager.

The i3-scrot command has multiple options that can be used to customize the screenshot process:

- "-s" allows the user to select a specific area of the screen to capture.
- "-f" saves the screenshot as a file in the home directory.
- "-cd" uses the clipboard to save the screenshot to the clipboard rather than a file.
- "-q" sets the quality of the screenshot. The value can range from 1 to 100, with 100 being the highest quality.
- "-t" adds a timestamp to the filename of the screenshot.

An example of using the i3-scrot command with options would be:

i3-scrot -s -f -q 80 -t

This command would allow the user to select a specific area of the screen, save the screenshot as a file, set its quality to 80, and add a timestamp to the filename. 

## tldr 
 
> Wrapper script around the screenshot utility `scrot` for the i3 window manager.
> The default save location is `~/Pictures` and can be changed in `~/.config/i3-scrot.conf`.
> More information: <https://gitlab.manjaro.org/packages/community/i3/i3-scrot>.

- Capture a screenshot of the whole screen and save it to the default directory:

`i3-scrot`

- Capture a screenshot of the active window:

`i3-scrot --window`

- Capture a screenshot of a specific rectangular selection:

`i3-scrot --select`

- Capture a screenshot of the whole screen and copy it to the clipboard:

`i3-scrot --desk-to-clipboard`

- Capture a screenshot of the active window and copy it to the clipboard:

`i3-scrot --window-to-clipboard`

- Capture a screenshot of a specific selection and copy it to the clipboard:

`i3-scrot --select-to-clibpoard`

- Capture a screenshot of the active window after a delay of 5 seconds:

`i3-scrot --window {{5}}`
