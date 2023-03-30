# gh config 
## chatgpt 
The `gh config` command is used to configure and manage the settings for a GitHub CLI tool named "gh". This command is used to set different configurations options like default editor, default repository format, media type, command-line prompt, time format, and so on.

When you run the `gh config` command without any options, it will display the current settings of the gh tool on your system.

Here are some subcommands available with the `gh config` command:

- `gh config get`: This subcommand is used to get the current value of a particular configuration option. For example, `gh config get prompt` will display the current command-line prompt setting.

- `gh config set`: This subcommand is used to set the value of a particular configuration option. For example, `gh config set editor nano` will set the default editor to nano.

- `gh config unset`: This subcommand is used to remove a configuration option from the configuration file. For example, `gh config unset prompt` will remove the custom prompt from the configuration file.

Overall, the `gh config` command is an essential command to manage and customize the gh tool according to your preferences. 

## tldr 
 
> Change configuration for GitHub cli.
> More information: <https://cli.github.com/manual/gh_config>.

- Display what Git protocol is being used:

`gh config get git_protocol`

- Set protocol to SSH:

`gh config set git_protocol {{ssh}}`

- Use `delta` in side-by-side mode as the default pager for all `gh` commands:

`gh config set pager '{{delta --side-by-side}}'`

- Set text editor to Vim:

`gh config set editor {{vim}}`

- Reset to default text editor:

`gh config set editor {{""}}`

- Disable interactive prompts:

`gh config set prompt {{disabled}}`

- Set a specific configuration value:

`gh config set {{key}} {{value}}`
