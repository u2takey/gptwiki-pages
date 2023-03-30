# screen 
## chatgpt 
The `screen` command is a Linux utility that allows users to create multiple virtual terminals within a single terminal window or shell session. This can be useful for managing multiple tasks or sessions simultaneously, without the need to physically switch between them.

Some of the key features of the `screen` command include:

- Multi-user support: Multiple users can connect to the same screen session and collaborate on tasks or projects together. 
- Session management: Screen sessions can be detached and re-attached later, allowing users to disconnect from a session and then reconnect from a different location or device. 
- Window management: Screen sessions can have multiple windows, each running its own process, and users can switch between windows or split the screen into multiple panes for even more flexibility. 

Once the `screen` command is invoked, it will create a new screen session with one window. Users can then start working within that window, launching programs or commands as needed. To navigate between windows or sessions, users can use key commands such as Ctrl-a c (create a new window), Ctrl-a n (switch to the next window), or Ctrl-a d (detach from the current session). 

Overall, the `screen` command is a powerful tool for managing terminal sessions and can be particularly useful for users who need to work on multiple tasks or projects simultaneously, or who frequently need to disconnect and reconnect from sessions. 

## tldr 
 
> Hold a session open on a remote server. Manage multiple windows with a single SSH connection.
> See also `tmux` and `zellij`.
> More information: <https://manned.org/screen>.

- Start a new screen session:

`screen`

- Start a new named screen session:

`screen -S {{session_name}}`

- Start a new daemon and log the output to `screenlog.x`:

`screen -dmLS {{session_name}} {{command}}`

- Show open screen sessions:

`screen -ls`

- Reattach to an open screen:

`screen -r {{session_name}}`

- Detach from inside a screen:

`Ctrl + A, D`

- Kill the current screen session:

`Ctrl + A, K`

- Kill a detached screen:

`screen -X -S {{session_name}} quit`
