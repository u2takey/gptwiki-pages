# i3lock 
## chatgpt 
i3lock is a command-line tool in Linux that is used to lock the screen of the system to prevent unauthorized access when the system is idle. 

When the i3lock command is executed, it displays a black screen with a prompt for a password. Only after entering the correct password, the user can log in and access the system.

i3lock is often used as a privacy and security measure to protect sensitive information from unauthorized access. It works by locking the keyboard and mouse, thus preventing the user from interacting with the system until the correct password is provided.

This command offers several customization features, such as setting the background color or using a custom image as the lock screen background. There are also many alternative programs and customizations that can be used instead of i3lock, depending on the user's preferences and needs. 

## tldr 
 
> Simple screen locker built for the i3 window manager.
> More information: <https://i3wm.org/i3lock>.

- Lock the screen showing a white background:

`i3lock`

- Lock the screen with a simple color background (rrggbb format):

`i3lock --color {{0000ff}}`

- Lock the screen to a PNG background:

`i3lock --image {{path/to/file.png}}`

- Lock the screen and disable the unlock indicator (removes feedback on keypress):

`i3lock --no-unlock-indicator`

- Lock the screen and don't hide the mouse pointer:

`i3lock --pointer {{default}}`

- Lock the screen to a PNG background tiled over all monitors:

`i3lock --image {{path/to/file.png}} --tiling`

- Lock the screen and show the number of failed login attempts:

`i3lock --show-failed-attempts`
