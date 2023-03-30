# yapf 
## chatgpt 
YAPF (Yet Another Python Formatter) is a command-line tool for formatting Python code according to a set of predefined rules. It automatically reforms poorly formatted code to match the guidelines established in PEP 8, providing users with standardized code formatting suited for the Python programming language.

The yapf tool can format entire source code files, or individual code snippets, depending on the use case. The basic syntax of the yapf command is as follows:

```
yapf [options] [file or directory]
```
where options can be any of the following:

- `--help`: displays help information about the command
- `--style`: specifies the formatting style to apply (default is "pep8")
- `--in-place`: modifies the file(s) in place, rather than printing to stdout
- `--recursive`: applies formatting recursively to all Python files in the specified directory
- `--exclude`: excludes specific files or directories from the formatting process
- `--parallel`: specifies the number of processes to use for formatting

For example, to format a Python file named "example.py" in the current directory with yapf, using the default PEP 8 style, simply run the following command:

```
yapf example.py
```

To format all Python files in a directory and its subdirectories, use the `--recursive` option:

```
yapf --recursive /path/to/directory
```

By default, yapf prints the formatted output to stdout. To modify files in place, use the `--in-place` option:

```
yapf --in-place example.py
```

It is also possible to exclude files or directories from the formatting process by using the `--exclude` option:

```
yapf --recursive --exclude="*/test/*" /path/to/directory
``` 

## tldr 
 
> Python style guide checker.
> More information: <https://github.com/google/yapf>.

- Display a diff of the changes that would be made, without making them (dry-run):

`yapf --diff {{path/to/file}}`

- Format the file in-place and display a diff of the changes:

`yapf --diff --in-place {{path/to/file}}`

- Recursively format all Python files in a directory, concurrently:

`yapf --recursive --in-place --style {{pep8}} --parallel {{path/to/directory}}`
