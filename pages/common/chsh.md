# chsh 
## chatgpt 
The "chsh" command is used in Linux and Unix-based operating systems to change the default shell for a user account.

Syntax: chsh [options] [username]

Options:
- -s, --shell: Specifies the new shell to use for the user account.
- -h, --help: Shows help information about the command.
- -l, --list-shells: Shows a list of available shells on the system.

Example usage:

To change the default shell for a user "johndoe" to the "zsh" shell, use the following command:

chsh -s /bin/zsh johndoe

This command will prompt the user for their password and then change the default shell for the specified user to "zsh".

Note: The "-s" option followed by the path to the new shell is required for this command to work. Also, the user account must have permission to use the new shell for it to execute properly. 

## tldr 
 
> Change user's login shell.
> More information: <https://manned.org/chsh>.

- Set a specific login shell for the current user interactively:

`chsh`

- Set a specific login [s]hell for the current user:

`chsh -s {{path/to/shell}}`

- Set a login [s]hell for a specific user:

`chsh -s {{path/to/shell}} {{username}}`

- [l]ist available shells:

`chsh -l`
