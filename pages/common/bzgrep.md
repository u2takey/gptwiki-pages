# bzgrep 
## chatgpt 
The command "bzgrep" is a Unix/Linux command that is used to search for a pattern in a compressed file that has been compressed using the bzip2 algorithm. The command works in a similar way to the "grep" command, which is used to search for a pattern in a regular text file.

When using "bzgrep", the syntax of the command is as follows:

```
bzgrep <pattern> <filename.bz2>
```

In this command, "pattern" is the text that you are searching for, and "filename.bz2" is the name of the compressed file that you want to search.

When you run the "bzgrep" command, it will search for the pattern in the compressed file and return any lines that contain the pattern. If the file is very large, the output might be piped through a pager such as "less" to let you scroll through the results. 

The "bzgrep" command is a very useful tool for searching through large compressed files quickly and efficiently. It can save time and disk space by avoiding having to decompress entire files before searching for a specific pattern. 

## tldr 
 
> Find patterns in bzip2 compressed files using grep.
> More information: <https://manned.org/bzgrep>.

- Search for a pattern within a compressed file:

`bzgrep "{{search_pattern}}" {{path/to/file}}`

- Use extended regular expressions (supports `?`, `+`, `{}`, `()` and `|`), in case-insensitive mode:

`bzgrep --extended-regexp --ignore-case "{{search_pattern}}" {{path/to/file}}`

- Print 3 lines of context around, before, or after each match:

`bzgrep --{{context|before-context|after-context}}={{3}} "{{search_pattern}}" {{path/to/file}}`

- Print file name and line number for each match:

`bzgrep --with-filename --line-number "{{search_pattern}}" {{path/to/file}}`

- Search for lines matching a pattern, printing only the matched text:

`bzgrep --only-matching "{{search_pattern}}" {{path/to/file}}`

- Recursively search files in a bzip2 compressed tar archive for a pattern:

`bzgrep --recursive "{{search_pattern}}" {{path/to/tar/file}}`

- Search `stdin` for lines that do not match a pattern:

`cat {{/path/to/bz/compressed/file}} | bzgrep --invert-match "{{search_pattern}}"`
