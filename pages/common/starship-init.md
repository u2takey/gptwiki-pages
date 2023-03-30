# starship init 
## chatgpt 
The command "starship init" is used to initialize the Starship prompt, which is a customizable and minimal shell prompt that can be used with various shells such as Bash, PowerShell, Fish, Zsh, and more.

When you run the "starship init" command, it will generate a default configuration file (starship.toml) in your home directory or the current directory, depending on whether there is an existing configuration file in your home directory or not.

The default configuration file includes simple settings such as the prompt format, color scheme, and shell specific configuration. You can modify this configuration file to customize the Starship prompt according to your preferences.

Once you have initialized the Starship prompt and configured it, you can then activate it in your shell by adding the necessary shell configuration to your shell profile (e.g., .bashrc, .zshrc), which is typically done automatically when you install Starship using a package manager.

Overall, "starship init" is a convenient command that helps you get started with configuring and using Starship prompt in your shell. 

## tldr 
 
> Print shell integration code for starship.
> More information: <https://starship.rs>.

- Display the subcommand help:

`starship init --help`

- Print the starship integration code for the specified shell:

`starship init {{bash|elvish|fish|ion|powershell|tcsh|zsh}}`

- Append the `starship` integration code to `~/.bashrc`:

`starship init {{bash}} >> {{~/.bashrc}}`

- Append the `starship` integration code to `~/.zshrc`:

`starship init {{zsh}} >> {{~/.zshrc}}`
