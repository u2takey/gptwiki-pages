# wmctrl 
## chatgpt 
WMCTRL (Window Manager Control) is a command-line utility tool in Linux that allows you to interact with your desktop's window manager. 

The command syntax is as follows: 

```bash
wmctrl [options] [arguments...]
```

Here are some of the most commonly used options: 

- `-l` - List the open windows and their properties.
- `-a` - Activate the window with a given title.
- `-R` - Raise the window with a given title to the front.
- `-r` - Move or resize a window with a given title.
- `-h` - Display help information on WMCTRL.
- `-m` - Output information about the window manager and its capabilities.
- `-v` - Run WMCTRL in verbose mode.

Using these options, you can manipulate open windows, move them around, resize them, and more. You can also use WMCTRL to automate certain tasks, like launching specific applications and moving them to specific workspaces. 

## tldr 
 
> CLI for X Window Manager.
> More information: <https://manned.org/wmctrl>.

- List all windows, managed by the window manager:

`wmctrl -l`

- Switch to the first window whose (partial) title matches:

`wmctrl -a {{window_title}}`

- Move a window to the current workspace, raise it and give it focus:

`wmctrl -R {{window_title}}`

- Switch to a workspace:

`wmctrl -s {{workspace_number}}`

- Select a window and toggle fullscreen:

`wmctrl -r {{window_title}} -b toggle,fullscreen`

- Select a window a move it to a workspace:

`wmctrl -r {{window_title}} -t {{workspace_number}}`
