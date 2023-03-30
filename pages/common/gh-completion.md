# gh completion 
## chatgpt 
The `gh completion` command is a git command that prints bash completion setup scripts for the `gh` command. This command helps to enable auto-completion for `gh` commands, which can dramatically improve the efficiency and speed of command line usage.

Auto-completion is a feature in bash that allows the shell to automatically suggest matching commands and options as you type, saving time and effort for frequently-used commands.

When you run `gh completion`, it will output the completion script that you can append to your bash profile, such as `.bashrc`, so that every time you start a new terminal session, the `gh` command will be auto-completed for you when you start typing.

The completion script output by `gh completion` includes all of the available commands and options for `gh`, providing a full list of suggestions as you complete your command within the terminal. You can use the arrow keys to navigate and select options from the list displayed, or continue typing to refine the list.

In summary, the `gh completion` command is a powerful tool that provides auto-completion support for Bash users working with the `gh` command. It helps to save time and effort by providing suggestions and options as you type, making the command line experience more efficient and streamlined. 

## tldr 
 
> Generate shell completion scripts for GitHub CLI commands.
> More information: <https://cli.github.com/manual/gh_completion>.

- Display the subcommand help:

`gh completion`

- Print a completion script:

`gh completion --shell {{bash|zsh|fish|powershell}}`

- Append the `gh` completion script to `~/.bashrc`:

`gh completion --shell {{bash}} >> {{~/.bashrc}}`

- Append the `gh` completion script to `~/.zshrc`:

`gh completion --shell {{zsh}} >> {{~/.zshrc}}`
