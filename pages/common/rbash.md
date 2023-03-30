# rbash 
## chatgpt 
The `rbash` command is used to launch a restricted shell, also known as a "restricted Bash shell". 

A restricted shell limits the functionality of Bash and restricts the user's ability to execute certain commands and use certain features of the shell. This can be useful for providing a more secure environment for users who need limited access to the system.

The `rbash` command sets the shell to restricted mode by setting the environment variable `BASH_ENV` to the value of `$HOME/.bashrc`. This means that the `bashrc` file in the user's home directory will be executed when the shell is launched, and any restrictions or customizations in that file will be applied to the shell session.

Some of the restrictions that may be enforced by `rbash` include:

- disabling the execution of external commands (i.e. running commands not built into the shell)
- disabling the execution of shell functions
- disabling the use of certain shell built-ins (e.g. `cd`)
- preventing changes to environment variables

These restrictions may be customized by editing the `bashrc` file or by using the `set` command to enable or disable specific features within the shell.

Overall, the `rbash` command is used to launch a more secure and restricted version of the Bash shell, which can be useful for providing limited access to users or for enforcing certain security policies on a system. 

## tldr 
 
> Restricted Bash shell, equivalent to `bash --restricted`.
> Does not permit changing the working directory, redirecting command output, or modifying environment variables, among other things.
> See also `histexpand` for history expansion.
> More information: <https://www.gnu.org/software/bash/manual/html_node/The-Restricted-Shell>.

- Start an interactive shell session:

`rbash`

- Execute a command and then exit:

`rbash -c "{{command}}"`

- Execute a script:

`rbash {{path/to/script.sh}}`

- Execute a script, printing each command before executing it:

`rbash -x {{path/to/script.sh}}`

- Execute commands from a script, stopping at the first error:

`rbash -e {{path/to/script.sh}}`

- Read and execute commands from `stdin`:

`rbash -s`
