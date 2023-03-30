# history expansion 
## chatgpt 
History expansion is a feature in Unix/Linux shells that allows users to repeat and modify previously executed commands quickly and easily. It allows users to access and manipulate previously executed command lines and their arguments by specifying their history number or by using special characters and modifiers.

The history command is a built-in command in most Unix/Linux shells that displays the list of previously executed commands, along with their history number. Users can access this history list using the up and down arrow keys on their keyboard, or by typing the history command.

To use history expansion, users can prefix a command with an exclamation mark (!), followed by an event designator, which specifies the command line or event to recall from the history list. The event designator can be a history number, a string that matches part of a command line, or a symbol that represents a particular command or range of commands.

For example, typing !! in a shell will execute the previous command, !-2 will execute the command two steps back in the history, and !ls will execute the most recent command that starts with the string ls.

History expansion also supports modifiers that allow users to manipulate and modify the command line before executing it. For example, adding :p to the end of a command with an event designator will print the resulting command line, but not execute it.

Overall, history expansion is a powerful feature in Unix/Linux shells that can save users time and effort while working in the command line. 

## tldr 
 
> Reuse and expand the shell history in `sh`, `bash`, `zsh`, `rbash` and `ksh`.
> More information: <https://www.gnu.org/software/bash/manual/html_node/History-Interaction>.

- Run the previous command as root (`!!` is replaced by the previous command):

`sudo !!`

- Run a command with the last argument of the previous command:

`{{command}} !$`

- Run a command with the first argument of the previous command:

`{{command}} !^`

- Run the Nth command of the history:

`!{{n}}`

- Run the command `n` lines back in the history:

`!-{{n}}`

- Run the most recent command containing `string`:

`!?{{string}}?`

- Run the previous command, replacing `string1` with `string2`:

`^{{string1}}^{{string2}}^`

- Perform a history expansion, but print the command that would be run instead of actually running it:

`{{!-n}}:p`
