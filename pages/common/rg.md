# rg 
## chatgpt 
The 'rg' command stands for "ripgrep", a command-line tool used for searching through files and directories. 

Syntax: rg [options] PATTERN [PATH ...]

- PATTERN: The search pattern (either a regular expression or plain text) that ripgrep will use to search for matches.
- PATH: The file or directory that ripgrep will search for matches. Multiple paths can be specified to search in several directories at the same time.

Options:
- -i or --ignore-case: This option will make the search case-insensitive.
- -w or --word-regexp: This option will only match whole words, i.e. it will not return partial matches.
- -v or --invert-match: This option will invert the match, i.e. return all lines that do not match the pattern.
- -C NUM or --context NUM: This option will display NUM lines of context before and after the matching lines.
- -f FILE or --file FILE: This option will read the search patterns from FILE, which can contain multiple patterns, one per line.
- --hidden: This option will search hidden files and directories (those beginning with a dot).

When executed with these parameters, 'rg' will search the specified files/directories for the given pattern and output the lines that match (or don't match, if -v is used). It is a fast and efficient tool for searching large files and directories. 

## tldr 
 
> Ripgrep is a recursive line-oriented CLI search tool.
> Aims to be a faster alternative to `grep`.
> More information: <https://github.com/BurntSushi/ripgrep>.

- Recursively search the current directory for a regular expression:

`rg {{regular_expression}}`

- Search for regular expressions recursively in the current directory, including hidden files and files listed in `.gitignore`:

`rg --no-ignore --hidden {{regular_expression}}`

- Search for a regular expression only in a subset of directories:

`rg {{regular_expression}} {{set_of_subdirs}}`

- Search for a regular expression in files matching a glob (e.g. `README.*`):

`rg {{regular_expression}} --glob {{glob}}`

- Search for filenames that match a regular expression:

`rg --files | rg {{regular_expression}}`

- Only list matched files (useful when piping to other commands):

`rg --files-with-matches {{regular_expression}}`

- Show lines that do not match the given regular expression:

`rg --invert-match {{regular_expression}}`

- Search a literal string pattern:

`rg --fixed-strings -- {{string}}`
