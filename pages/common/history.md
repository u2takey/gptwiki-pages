# history 
## chatgpt 
The `history` command in Unix-based systems is used to display a list of the commands that have been executed in the current terminal session. It provides a chronological and numbered list of previously executed commands, including those that were executed in previous sessions. This feature is useful when you need to remember a previously executed command, as it helps to reduce the time spent in retyping a command that you recently used by referring to the command history.

When you run the `history` command, it will display a list of commands that have been executed, arranged with the most recent at the bottom of the list. By default, the `history` command in Unix displays only the most recent 100 commands that were executed. You can adjust the number of commands that history displays by modifying the `HISTSIZE` environment variable. For example, if you want to see the last 20 commands that you typed, you can use the command `history 20`.

Each command in the history list is assigned a unique number which can be used to rerun the command. You can repeat any command by typing `!n`, where `n` is the number assigned to the command in the list. For example, if you want to rerun the 7th command in the history list, you can type `!7`.

The `history` command can also be used with additional options and flags to display more detailed information. For example, the `-c` flag can clear the entire history list, while the `-a` flag can be used to add commands to the history list as soon as they are executed. You can view all the available options by typing `man history` to see the full documentation of the `history` command. 

## tldr 
 
> Command-line history.
> More information: <https://www.gnu.org/software/bash/manual/html_node/Bash-History-Builtins.html>.

- Display the commands history list with line numbers:

`history`

- Display the last 20 commands (in `zsh` it displays all commands starting from the 20th):

`history {{20}}`

- Clear the commands history list (only for current `bash` shell):

`history -c`

- Overwrite history file with history of current `bash` shell (often combined with `history -c` to purge history):

`history -w`

- Delete the history entry at the specified offset:

`history -d {{offset}}`
