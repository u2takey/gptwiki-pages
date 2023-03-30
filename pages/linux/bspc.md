# bspc 
## chatgpt 
`bspc` is a command for managing windows and workspaces in a multi-monitor environment using Binary Space Partitioning. It is a part of the BSPWM (Binary Space Partitioning Window Manager) project, which is a tiling window manager for Linux that arranges windows in a non-overlapping layout on the screen.

The `bspc` command provides a wide range of options for managing windows and workspaces, including:

- `bspc monitor`: This command is used to identify and view the properties of each connected monitor, including its name, status, resolution, and refresh rate.

- `bspc rule`: This command allows you to set rules that define how windows are treated when they are created or moved. This can include setting the size or position of new windows, or specifying which workspace they should appear on.

- `bspc node`: This command is used to view and manipulate the properties of individual windows, including their position, size, and the workspace they are on. You can move and resize windows, as well as set their state to floating or fullscreen.

- `bspc desktop`: This command is used to view and manipulate individual workspaces. You can switch between workspaces or move windows from one workspace to another. You can also define custom names for each workspace.

Overall, `bspc` is a powerful command that provides a great deal of flexibility and control over your workspace and windows. It is ideal for power users who need to manage large numbers of windows across multiple monitors. 

## tldr 
 
> A tool to control `bspwm`.
> More information: <https://github.com/baskerville/bspwm>.

- Define two virtual desktop:

`bspc monitor --reset-desktops {{1}} {{2}}`

- Focus the given desktop:

`bspc desktop --focus {{number}}`

- Close the windows rooted at the selected node:

`bspc node --close`

- Send the selected node to the given desktop:

`bspc node --to-desktop {{number}}`

- Toggle full screen mode for the selected node:

`bspc node --state ~fullscreen`
