# zsh 
## chatgpt 
The `zsh` command is used to launch the Z shell, a Unix shell that is an extended version of the Bourne shell (sh) with additional features and syntax. The name "zsh" stands for "Z shell."

When you run the `zsh` command, it will start a new shell session in your terminal with the Z shell as its default shell. This means that any commands you type into the terminal will be interpreted and executed by the Z shell.

The Z shell has many features that make it a popular choice among power users and developers. Some of its key features include:

- Tab completion: The Z shell has a powerful tab completion mechanism that can complete commands, options, and file names based on context and history.

- File globbing: The Z shell has advanced file globbing syntax that allows you to select and manipulate files based on patterns.

- Prompt customization: The Z shell has a flexible and customizable prompt system that allows you to display information and colors in the terminal prompt.

- Command aliases: The Z shell allows you to define short aliases for commonly used commands, making it easier to type and remember them.

Overall, the `zsh` command is a powerful tool for anyone who wants to use the Z shell as their default Unix shell. By launching the Z shell with this command, you can take advantage of its advanced features and syntax to improve your productivity and efficiency in the terminal. 

## tldr 
 
> Z SHell, a Bash-compatible command-line interpreter.
> See also: `bash`, `histexpand`.
> More information: <https://www.zsh.org>.

- Start an interactive shell session:

`zsh`

- Execute specific [c]ommands:

`zsh -c "{{echo Hello world}}"`

- Execute a specific script:

`zsh {{path/to/script.zsh}}`

- Check a specific script for syntax errors without executing it:

`zsh --no-exec {{path/to/script.zsh}}`

- Execute specific commands from stdin:

`{{echo Hello world}} | zsh`

- Execute a specific script, printing each command in the script before executing it:

`zsh --xtrace {{path/to/script.zsh}}`

- Start an interactive shell session in verbose mode, printing each command before executing it:

`zsh --verbose`

- Execute a specific command inside `zsh` with disabled glob patterns:

`noglob {{command}}`
