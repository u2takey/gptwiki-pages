# qtile 
## chatgpt 
`qtile` is a Python-based window manager for X Window System. It provides a highly customizable and programmable interface for managing windows with a focus on keyboard shortcuts and scriptability.

When executed as a command, `qtile` starts the window manager and launches the default configuration file located at `~/.config/qtile/config.py`. This file defines the layout and behavior of the window manager and can be edited to modify the behavior of the window manager.

Once `qtile` is running, users can interact with it using keyboard shortcuts to perform actions such as opening and closing windows, switching between workspaces, resizing and moving windows, and more. The `qtile` command can be used to manage the window manager, such as restarting, reloading the configuration file, or quitting the window manager.

Overall, `qtile` provides a powerful and flexible window management solution for Linux users who want to customize their desktop environment to fit their specific needs and workflow. 

## tldr 
 
> A full-featured, hackable tiling window manager written and configured in Python.
> More information: <https://docs.qtile.org/en/latest/manual/commands/shell/index.html>.

- Start the window manager, if it is not running already (should ideally be run from `.xsession` or similar):

`qtile start`

- Check the configuration file for any compilation errors (default location is  `~/.config/qtile/config.py`):

`qtile check`

- Show current resource usage information:

`qtile top --force`

- Open the program `xterm` as a floating window on the group named `test-group`:

`qtile run-cmd --group {{test-group}} --float {{xterm}}`

- Restart the window manager:

`qtile cmd-obj --object cmd --function restart`
