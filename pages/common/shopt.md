# shopt 
## chatgpt 
The shopt command is used in Linux and Unix operating systems to manipulate various shell options. The command is used to set or unset options that control the behavior of the shell under certain conditions. The shopt command is used with one or more of the following options:

- -s - to set an option
- -u - to unset an option

Some common options that can be manipulated using the shopt command are:

- autocd - if set, enables automatic changing of directory to the one entered as a command
- cdable_vars - if set, enables changing to a directory using a variable name
- checkhash - if set, the shell checks the command hash table before executing external commands
- globstar - if set, enables the "**" glob pattern to match all files and directories recursively
- nocaseglob - if set, makes the shell glob pattern matching case-insensitive

To use the shopt command, you simply enter "shopt" followed by the option you want to set or unset, and the name of the option. For example, to enable the autocd option, you would enter:

shopt -s autocd

To unset the option, you would enter:

shopt -u autocd

Using the shopt command allows you to customize your shell's behavior to better suit your needs and preferences, and can make working with the shell more efficient and convenient. 

## tldr 
 
> Manage Bash shell options: variables (stored in `$BASHOPTS`) that control behavior specific to the Bash shell.
> Generic POSIX shell variables (stored in `$SHELLOPTS`) are managed with the `set` command instead.
> More information: <https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html>.

- List of all settable options and whether they are set:

`shopt`

- Set an option:

`shopt -s {{option_name}}`

- Unset an option:

`shopt -u {{option_name}}`

- Print a list of all options and their status formatted as runnable `shopt` commands:

`shopt -p`

- Show help for the command:

`help shopt`
