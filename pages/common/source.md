# source 
## chatgpt 
The `source` command is a shell built-in command that executes the content of a shell script file in the current shell context. It is also used to run commands in the current shell session.

When you run a script using the `source` command, any changes made to the environment variables, aliases, or functions in the script will be applied to the current shell's environment directly.

The `source` command is sometimes also called the `dot` command or `period` command, and its syntax is pretty simple. Here's how it works:

```
source script_name.sh
```

The above command runs the shell script `script_name.sh` in the current shell context.

The `source` command is often used when you need to set environment variables or define functions that are used by other scripts or programs. By sourcing a script, you avoid the need to export variables or functions since they're defined directly in the parent shell context.

Overall, the `source` command is a powerful tool for running shell scripts and defining environment variables in a way that's easy and efficient. 

## tldr 
 
> Execute commands from a file in the current shell.
> More information: <https://manned.org/source>.

- Evaluate contents of a given file:

`source {{path/to/file}}`

- Evaluate contents of a given file (alternatively replacing `source` with `.`):

`. {{path/to/file}}`
