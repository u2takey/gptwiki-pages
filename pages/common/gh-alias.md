# gh alias 
## chatgpt 
The `gh alias` command is a command in the GitHub CLI tool (also known as `gh`) that allows you to create and manage aliases for frequently used commands.

When you run the `gh alias` command, you are presented with several subcommands that you can use to manage your aliases. These include:

- `gh alias set`: This subcommand allows you to create a new alias or overwrite an existing one. You specify the name of the alias and the command that it should map to. For example, you could create an alias named `pr` that maps to the `pull-request` command.

- `gh alias list`: This subcommand lists all of your currently defined aliases.

- `gh alias delete`: This subcommand allows you to delete an existing alias by specifying its name.

- `gh alias help`: This subcommand provides help documentation on how to use the `gh alias` command.

Aliases can be very helpful in speeding up your workflow by allowing you to quickly run complex or lengthy commands with a single short alias command. Additionally, aliases can be shared across your team or even across your organization to standardize frequently used commands. 

## tldr 
 
> Manage GitHub CLI command aliases from the command-line.
> More information: <https://cli.github.com/manual/gh_alias>.

- Display the subcommand help:

`gh alias`

- List all the aliases `gh` is configured to use:

`gh alias list`

- Create a `gh` subcommand alias:

`gh alias set {{pv}} '{{pr view}}'`

- Set a shell command as a `gh` subcommand:

`gh alias set --shell {{alias_name}} {{command}}`

- Delete a command shortcut:

`gh alias delete {{alias_name}}`
