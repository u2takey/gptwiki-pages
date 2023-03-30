# env 
## chatgpt 
The "env" command is a shell command in Linux and Unix-based operating systems that displays or sets environment variables. 

When used without any arguments, the "env" command displays a list of all the environment variables currently set in the shell session. This includes variables such as the user's home directory, the current working directory, the default editor, and other settings.

The "env" command can also be used with arguments to set environment variables. For example, the command "env LANG=en_US.UTF-8" sets the LANG environment variable to the value "en_US.UTF-8". This can be useful when running programs that require certain environment variables to be set.

Overall, the "env" command is a useful tool for managing and viewing environment variables in a shell session. 

## tldr 
 
> Show the environment or run a program in a modified environment.
> More information: <https://www.gnu.org/software/coreutils/env>.

- Show the environment:

`env`

- Run a program. Often used in scripts after the shebang (#!) for looking up the path to the program:

`env {{program}}`

- Clear the environment and run a program:

`env -i {{program}}`

- Remove variable from the environment and run a program:

`env -u {{variable}} {{program}}`

- Set a variable and run a program:

`env {{variable}}={{value}} {{program}}`

- Set multiple variables and run a program:

`env {{variable1}}={{value}} {{variable2}}={{value}} {{variable3}}={{value}} {{program}}`
