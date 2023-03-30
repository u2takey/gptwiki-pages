# zellij 
## chatgpt 
Zellij is a terminal multiplexer and workspace manager that allows users to work on multiple tasks in the same terminal window or multiple terminal windows simultaneously. It is an open-source software that is available for Linux and macOS.

To use Zellij, you first need to install it on your system. You can install it using your system's package manager or by building it from source. Once installed, you can run it by entering the command "zellij" in the terminal.

After running the command, you will be presented with a Zellij workspace that is divided into panes. Each pane can contain a different terminal session or application, allowing you to work on multiple tasks simultaneously. You can navigate between panes using the keyboard shortcuts or by clicking on them using the mouse.

Zellij also offers several customization options, such as changing the background and font color, resizing panes, and creating custom keybindings. You can configure these settings by editing the configuration file located in the "~/.config/zellij" directory.

Overall, Zellij is a powerful tool that can streamline your workflow and improve your productivity by allowing you to work on multiple tasks in a single terminal workspace. 

## tldr 
 
> Terminal multiplexer with batteries included.
> See also `tmux` and `screen`.
> More information: <https://zellij.dev/documentation/>.

- Start a new named session:

`zellij --session {{name}}`

- List existing sessions:

`zellij list-sessions`

- Attach to the most recently used session:

`zellij attach`

- Open a new pane (inside a zellij session):

`Alt + N`

- Detach from the current session (inside a zellij session):

`Ctrl + N, D`
