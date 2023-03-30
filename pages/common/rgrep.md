# rgrep 
## chatgpt 
The command `rgrep` is a combination of two commands: `grep` and `r` (short for recursive). The `grep` command is used to search for patterns in files, while the `r` option tells it to search recursively through directories and subdirectories.

Here is the syntax:

```
rgrep [OPTIONS] PATTERN [FILE...]
```

- `OPTIONS`: Optional arguments that modify the behavior of the command. Some common ones include `-i` (ignore case), `-n` (print line numbers), and `-v` (print lines that do not match).
- `PATTERN`: The pattern to search for in the files. This can be a regular expression or a string.
- `FILE...`: The file or files to search in. If none are specified, `rgrep` will search in all files in the current directory and its subdirectories.

Here is an example:

```
rgrep -i "hello world" *.txt
```

This command will search for the string "hello world" in all `.txt` files in the current directory and its subdirectories, ignoring case. 

## tldr 
 
> Recursively find patterns in files using regular expressions.
> Equivalent to `grep -r`.
> More information: <https://www.gnu.org/software/grep/manual/grep.html>.

- Recursively search for a pattern in the current working directory:

`rgrep "{{search_pattern}}"`

- Recursively search for a case-insensitive pattern in the current working directory:

`rgrep --ignore-case "{{search_pattern}}"`

- Recursively search for an extended regular expression pattern (supports `?`, `+`, `{}`, `()` and `|`) in the current working directory:

`rgrep --extended-regexp "{{search_pattern}}"`

- Recursively search for an exact string (disables regular expressions) in the current working directory:

`rgrep --fixed-strings "{{exact_string}}"`

- Recursively search for a pattern in a specified directory (or file):

`rgrep "{{search_pattern}}" {{path/to/file_or_directory}}`
