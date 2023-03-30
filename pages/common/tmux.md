# tmux 
## chatgpt 
The "tmux" command is used to launch the tmux terminal multiplexer program. Tmux is a powerful tool that allows users to create multiple terminal sessions within a single screen or window, each with its own set of panes, tabs, and other features. 

When you run the "tmux" command, it will launch a new tmux session with a single window, containing one pane. You can then use various keyboard commands to create new windows and panes, split existing panes, move between panes and windows, and more. 

Some common tmux commands include: 

- "Ctrl-b c": Create a new window
- "Ctrl-b n": Move to the next window
- "Ctrl-b %": Split the current pane vertically
- "Ctrl-b ": Split the current pane horizontally
- "Ctrl-b arrow key": Move to the pane in the specified direction
- "Ctrl-b d": Detach the tmux session and return to the normal terminal

Tmux can be a bit daunting for beginners, but it's a powerful tool that can greatly enhance your productivity and workflow once you get the hang of it. 

## tldr 
 
> Terminal multiplexer. It allows multiple sessions with windows, panes, and more.
> See also `zellij` and `screen`.
> More information: <https://github.com/tmux/tmux>.

- Start a new session:

`tmux`

- Start a new named session:

`tmux new -s {{name}}`

- List existing sessions:

`tmux ls`

- Attach to the most recently used session:

`tmux attach`

- Detach from the current session (inside a tmux session):

`Ctrl-B d`

- Create a new window (inside a tmux session):

`Ctrl-B c`

- Switch between sessions and windows (inside a tmux session):

`Ctrl-B w`

- Kill a session by name:

`tmux kill-session -t {{name}}`
