# egrep 
## chatgpt 
`egrep` is a command in Unix-based operating systems that is used to search for text patterns using regular expressions in a file or files. It is essentially an extended version of the `grep` command that provides additional functionality.

The syntax for using `egrep` is as follows:

```
egrep [options] pattern [file ...]
```

Here, `pattern` refers to the regular expression that is used to search for text in the specified file(s).

Some common options that can be used with the `egrep` command include:

- `-i`: Ignore case while searching for the pattern
- `-v`: Invert the search, i.e., display lines that do not contain the pattern
- `-n`: Display the line number along with the matching line
- `-c`: Display only the count of matching lines

For example, the command `egrep -i 'hello' file.txt` will search for the string "hello" in the file `file.txt`, ignoring case.

Regular expressions can be used to search for complex patterns such as strings that begin with or contain certain characters, specific word patterns, or even entire sentences. This allows for powerful and flexible searching and filtering of files. 

## tldr 
 
> Find patterns in files using extended regular expression (supports `?`, `+`, `{}`, `()` and `|`).
> More information: <https://manned.org/egrep>.

- Search for a pattern within a file:

`egrep "{{search_pattern}}" {{path/to/file}}`

- Search for a pattern within multiple files:

`egrep "{{search_pattern}}" {{path/to/file1}} {{path/to/file2}} {{path/to/file3}}`

- Search `stdin` for a pattern:

`cat {{path/to/file}} | egrep {{search_pattern}}`

- Print file name and line number for each match:

`egrep --with-filename --line-number "{{search_pattern}}" {{path/to/file}}`

- Search for a pattern in all files recursively in a directory, ignoring binary files:

`egrep --recursive --binary-files={{without-match}} "{{search_pattern}}" {{path/to/directory}}`

- Search for lines that do not match a pattern:

`egrep --invert-match "{{search_pattern}}" {{path/to/file}}`
