# dash 
## chatgpt 
`dash` is a command that launches the Debian Almquist Shell, which is a UNIX shell that is similar to the Bourne shell but includes additional features such as job control and command line editing. 

When the `dash` command is executed, a new shell will be created and the user will be presented with a command prompt where they can enter commands to be executed within the shell. These commands may include built-in shell commands such as cd (change directory), echo (print text to the screen), and exit (exit the shell), as well as external commands that have been installed on the system.

One important thing to note about `dash` is that it is designed to be a minimal shell that is fast and efficient, which makes it well-suited for use in scripts and other situations where speed is a priority. However, because it does not include some of the more advanced features found in other shells (such as Bash), it may not be as user-friendly for interactive use.

Overall, the `dash` command is a versatile tool that provides users with a lightweight shell that can be used for a variety of tasks, from running simple commands to scripting complex tasks. 

## tldr 
 
> Debian Almquist Shell, a modern, POSIX-compliant implementation of `sh` (not Bash-compatible).
> More information: <https://manned.org/dash>.

- Start an interactive shell session:

`dash`

- Execute specific [c]ommands:

`dash -c "{{echo 'dash is executed'}}"`

- Execute a specific script:

`dash {{path/to/script.sh}}`

- Check a specific script for syntax errors:

`dash -n {{path/to/script.sh}}`

- Execute a specific script while printing each command before executing it:

`dash -x {{path/to/script.sh}}`

- Execute a specific script and stop at the first [e]rror:

`dash -e {{path/to/script.sh}}`

- Execute specific commands from `stdin`:

`{{echo "echo 'dash is executed'"}} | dash`
