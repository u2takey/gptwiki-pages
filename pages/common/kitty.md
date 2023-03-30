# kitty 
## chatgpt 
The "kitty" command is typically used as a terminal emulator program for Linux and other Unix-like operating systems. When executed, it opens a graphical terminal window that allows users to interact with the command line interface of their system.

Some of the key features of the Kitty terminal emulator include support for Unicode characters, keyboard shortcuts for copy/paste functions, configurable appearance and layout options, and support for multiple tabs and windows.

To use the Kitty command, you simply need to open a terminal window or console and type "kitty" followed by any command-line arguments or flags that you want to use. For example, you could enter "kitty -o font_size=16" to specify a specific font size when the terminal window opens.

Overall, the Kitty command can be a useful tool for developers, system administrators, and other users who regularly work with command line interfaces and need a reliable, fully-featured terminal emulator. 

## tldr 
 
> A fast, feature-rich, GPU based terminal emulator.
> More information: <https://sw.kovidgoyal.net/kitty/>.

- Open a new terminal:

`kitty`

- Open a terminal with the specified title for the window:

`kitty --title "{{title}}"`

- Start the theme-chooser builtin:

`kitty +kitten themes`

- Display an image in the terminal:

`kitty +kitten icat {{path/to/image}}`

- Copy the contents of `stdin` to the clipboard:

`echo {{example}} | kitty +kitten clipboard`
