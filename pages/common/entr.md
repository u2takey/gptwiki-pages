# entr 
## chatgpt 
The `entr` command is a utility for monitoring changes in files and executing commands in response to those changes. 

When you run `entr`, you provide it with a command to execute as its argument. `entr` will then wait for changes in the current directory (and all subdirectories). When a change is detected, `entr` will execute the provided command.

For example, suppose you have a Python script called `myscript.py`, which you want to execute every time you save changes to it. You could use `entr` as follows:

```
$ ls myscript.py | entr python myscript.py
```

Here, we use `ls` to send the filename of `myscript.py` to `entr`. Then, we tell `entr` to execute the command `python myscript.py` every time a change is detected in the file.

You can also monitor multiple files and execute a more complex command. For example, to run a test suite every time files change in the `tests/` directory or in any Python file in the project, you could use:

```
$ ls **/*.py tests/* | entr pytest tests/
```

The `**` matches any subdirectory, so this command will monitor all Python files in the project. When a change is detected in one of these files or in the `tests/` directory itself, `entr` will run the `pytest` command, which will execute the test suite. 

## tldr 
 
> Run arbitrary commands when files change.
> More information: <https://manned.org/entr>.

- Rebuild with `make` if any file in any subdirectory changes:

`{{ag -l}} | entr {{make}}`

- Rebuild and test with `make` if any `.c` source files in the current directory change:

`{{ls *.c}} | entr {{'make && make test'}}`

- Send a `SIGTERM` to any previously spawned ruby subprocesses before executing `ruby main.rb`:

`{{ls *.rb}} | entr -r {{ruby main.rb}}`

- Run a command with the changed file (`/_`) as an argument:

`{{ls *.sql}} | entr {{psql -f}} /_`
