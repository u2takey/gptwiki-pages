# zgrep 
## chatgpt 
`zgrep` is a command in Linux and Unix operating systems that allows you to search for a pattern in a compressed file. It works similarly to the `grep` command, but is designed to work with files that have been compressed using the gzip utility.

The `zgrep` command takes the following syntax:

```
zgrep [OPTIONS] PATTERN [FILES...]
```

Here's what each part of the command means:

- `zgrep`: The name of the command itself.
- `[OPTIONS]`: Optional flags that modify the behavior of the command. We'll cover some of the most common ones below.
- `PATTERN`: The search string that you want to find in the compressed file(s). This can be a regular expression.
- `[FILES...]`: One or more compressed files that you want to search. These files should be in gzip format (with a .gz extension).

Here are some common options you can use with `zgrep`:

- `-i`: Ignore case when searching.
- `-l`: Print only the names of the files that match the search pattern.
- `-n`: Print the line number of each match.
- `-r`: Recursively search through all files in a directory (useful for searching through log files, for example).
- `-v`: Invert the search, showing lines that do not match the search pattern.

Here are some examples of how to use the `zgrep` command:

```
zgrep "error" logfile.gz
```

This searches for the word "error" in the compressed file logfile.gz and prints out any lines that contain that word.

```
zgrep -i "error" *.gz
```

This searches for the word "error" in all compressed files in the current directory (with a .gz extension), and ignores case when searching.

```
zgrep -l "error" *.gz
```

This searches for the word "error" in all compressed files in the current directory (with a .gz extension) and prints out only the names of the files that contain that word.

Overall, `zgrep` is a powerful tool for searching through compressed files quickly and easily, especially when dealing with large log files or other text files that are regularly compressed. 

## tldr 
 
> Grep text patterns from files within compressed file (equivalent to grep -Z).
> More information: <https://manned.org/zgrep>.

- Grep a pattern in a compressed file (case-sensitive):

`zgrep {{pattern}} {{path/to/compressed/file}}`

- Grep a pattern in a compressed file (case-insensitive):

`zgrep -i {{pattern}} {{path/to/compressed/file}}`

- Output count of lines containing matched pattern in a compressed file:

`zgrep -c {{pattern}} {{path/to/compressed/file}}`

- Display the lines which don’t have the pattern present (Invert the search function):

`zgrep -v {{pattern}} {{path/to/compressed/file}}`

- Grep a compressed file for multiple patterns:

`zgrep -e "{{pattern_1}}" -e "{{pattern_2}}" {{path/to/compressed/file}}`

- Use extended regular expressions (supporting `?`, `+`, `{}`, `()` and `|`):

`zgrep -E {{regular_expression}} {{path/to/file}}`

- Print 3 lines of [C]ontext around, [B]efore, or [A]fter each match:

`zgrep -{{C|B|A}} {{3}} {{pattern}} {{path/to/compressed/file}}`
