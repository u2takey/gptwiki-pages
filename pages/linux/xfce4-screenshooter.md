# xfce4-screenshooter 
## chatgpt 
The `xfce4-screenshooter` command is a screenshot utility for the Xfce desktop environment. It allows you to take screenshots of your desktop or individual windows in various ways, including:

- Full-screen screenshot: captures the entire screen and saves it as an image file.
- Window screenshot: captures the specified window and saves it as an image file.
- Rectangular screenshot: captures a selected rectangular area of the screen and saves it as an image file.
- Delayed screenshot: captures the specified element after a certain delay (e.g., 5 seconds), which allows you to prepare for the screenshot by opening menus, pop-ups, etc.

This command can be executed in the terminal, or through the Xfce menu or keyboard shortcuts. The screenshots are saved in your home directory by default, in the Pictures folder. The file format of the screenshot can be changed through the Preferences menu.

In summary, `xfce4-screenshooter` is a versatile tool for capturing screenshots in the Xfce desktop environment, and it offers several options for customizing the screenshots to meet your needs. 

## tldr 
 
> The XFCE4 screenshot tool.
> More information: <https://docs.xfce.org/apps/xfce4-screenshooter/start>.

- Launch the screenshooter GUI:

`xfce4-screenshooter`

- Take a screenshot of the entire screen and launch the GUI to ask how to proceed:

`xfce4-screenshooter --fullscreen`

- Take a screenshot of the entire screen and save it in the specified directory:

`xfce4-screenshooter --fullscreen --save {{path/to/directory}}`

- Wait some time before taking the screenshot:

`xfce4-screenshooter --delay {{seconds}}`

- Take a screenshot of a region of the screen (select using the mouse):

`xfce4-screenshooter --region`

- Take a screenshot of the active window, and copy it to the clipboard:

`xfce4-screenshooter --window --clipboard`

- Take a screenshot of the active window, and open it with a chosen program:

`xfce4-screenshooter --window --open {{gimp}}`
