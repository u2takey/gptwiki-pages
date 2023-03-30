# alias 
## chatgpt 
The command "alias" is used to create a shortcut for a command or a series of commands. When using an alias, typing the alias in the terminal will execute the entire set of commands associated with it.

Syntax:
alias [alias_name]='command'

For example, let's say we want to create an alias for "ls -alh" command, we can use the following syntax:

alias lh='ls -alh'

Now, every time we type "lh" in the terminal, it will execute the "ls -alh" command.

We can also view all the aliases currently set on our system by typing the "alias" command without any options.

Overall, the alias command is useful for saving time by creating shortcuts for frequently used commands. 

## tldr 
 
> Creates aliases -- words that are replaced by a command string.
> Aliases expire with the current shell session unless defined in the shell's configuration file, e.g. `~/.bashrc`.
> More information: <https://tldp.org/LDP/abs/html/aliases.html>.

- List all aliases:

`alias`

- Create a generic alias:

`alias {{word}}="{{command}}"`

- View the command associated to a given alias:

`alias {{word}}`

- Remove an aliased command:

`unalias {{word}}`

- Turn `rm` into an interactive command:

`alias {{rm}}="{{rm --interactive}}"`

- Create `la` as a shortcut for `ls --all`:

`alias {{la}}="{{ls --all}}"`
