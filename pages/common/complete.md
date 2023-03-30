# complete 
## chatgpt 
The "complete" command is used in the Linux/Unix shell to define how commands should be completed by the shell's auto-completion feature. When a user types in part of a command or file name and presses the Tab key, the shell will attempt to complete the input based on the defined completion rules.

The syntax for the complete command is:

```complete [OPTIONS] COMMAND```

Here, "OPTIONS" can be used to specify various options for the completion. Some common options include:

- "-r": removes any existing completion for the specified command
- "-p": displays the current completion for the specified command

"COMMAND" should be the name of the command for which you want to define completion behavior. You can also use "*" to define completion rules for all commands.

After specifying the options and command name, you can then define the completion behavior using various arguments. Some common arguments include:

- "-W WORDS": defines a list of possible completion words separated by spaces
- "-f": completes filenames instead of command names
- "-o OPTION": specifies additional options for the completion, such as "nospace" to suppress adding a space after the completed word

For example, to define completion rules for the "git" command, you might use:

```complete -W "add commit push branch checkout" git```

This means that when a user types "git" and then presses Tab, the shell will suggest possible completion options from the provided list. If the user types "git a" and then presses Tab, the shell will complete to "git add", since "add" is the only option that starts with "a". 

## tldr 
 
> Provides argument autocompletion to shell commands.
> More information: <https://www.gnu.org/software/bash/manual/html_node/Programmable-Completion-Builtins.html>.

- Apply a function that performs autocompletion to a command:

`complete -F {{function}} {{command}}`

- Apply a command that performs autocompletion to another command:

`complete -C {{autocomplete_command}} {{command}}`

- Apply autocompletion without appending a space to the completed word:

`complete -o nospace -F {{function}} {{command}}`
