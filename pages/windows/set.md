# set 
## chatgpt 
The "set" command is a command that is commonly used in various operating systems such as Windows, Unix, and Linux. The command has different functions, depending on the context in which it is used.

In general, the "set" command is used to manipulate environment variables. Environment variables are a set of values that define certain properties of the operating system and its environment. These variables can be used to store information such as the path to executables, the default editor, or the location of specific files or directories.

Using the "set" command, you can view the current environment variables, create new variables or modify existing variables. The syntax of the command may vary depending on the operating system, but some of the most common options and arguments include:

- "-a": Displays all environment variables and their values.
- "-x": Displays the export commands needed to recreate the current environment variables.
- "NAME=VALUE": Creates a new environment variable with the specified name and value.
- "NAME=": Deletes the environment variable with the specified name.

In summary, the "set" command is a versatile tool for managing environment variables in an operating system. It allows users to customize their environment and tailor it to their specific needs. 

## tldr 
 
> Display or set environment variables for the current instance of CMD.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/set>.

- List all current environment variables:

`set`

- Set an environment variable to a specific value:

`set {{name}}={{value}}`

- List environment variables starting with the specified string:

`set {{name}}`

- Prompt the user for a value for the specified variable:

`set /p {{name}}={{prompt_string}}`
