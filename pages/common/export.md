# export 
## chatgpt 
The `export` command is used in Unix-based operating systems to set or modify the value of an environment variable for the current shell session and all its child processes. When you export a variable with `export VAR_NAME=value`, the variable `VAR_NAME` will become available to all child processes, such as shell scripts, executed from the current shell session.

Here's a breakdown of the `export` command:

- Syntax: `export VAR_NAME=[value]`
- `VAR_NAME` is the name of the environment variable you want to set, and `value` is the value you want to assign to it. If you omit the `value` parameter, the variable is unset and its value is empty.
- Once you've exported a variable, you can access its value from within the current shell or any child processes invoked from that shell. For example, if you run `export MY_VAR="Hello, World!"`, you can then access `$MY_VAR` in subsequent commands or scripts to get the value "Hello, World!".
- You can also use the `env` command to list all currently exported environment variables on your system.
- Note that exported variables are not persistent across system reboots or new shell sessions. If you want to set a variable permanently, you should add it to your shell's configuration file (e.g. `.bashrc` or `.zshrc`).

Here are a few examples of how to use the `export` command:

1. Exporting a variable with a value:
```
$ export MY_VAR="Hello, World!"
$ echo $MY_VAR
Hello, World!
```

2. Exporting a variable without a value (unsetting it):
```
$ export MY_VAR=
$ echo $MY_VAR

```

3. Listing all currently exported variables:
```
$ env
SHELL=/bin/bash
USER=jdoe
HOME=/home/jdoe
MY_VAR=Hello, World!
...
```

4. Exporting a variable to a child process (in this case, a Python script):
```
$ export MY_VAR="Hello, World!"
$ python my_script.py
```

In the example above, the `MY_VAR` variable is exported to the Python interpreter environment, so it can be accessed by the `my_script.py` script. 

## tldr 
 
> Command to mark shell variables in the current environment to be exported with any newly forked child processes.
> More information: <https://www.gnu.org/software/bash/manual/bash.html#index-export>.

- Set a new environment variable:

`export {{VARIABLE}}={{value}}`

- Remove an environment variable:

`export -n {{VARIABLE}}`

- Mark a shell function for export:

`export -f {{FUNCTION_NAME}}`

- Append something to the PATH variable:

`export PATH=$PATH:{{path/to/append}}`
