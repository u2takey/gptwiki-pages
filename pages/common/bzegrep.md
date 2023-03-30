# bzegrep 
## chatgpt 
The command "bzegrep" is used to search for a pattern in one or more bzip2-compressed files. It works like the "egrep" command, but is specifically designed to handle compressed files.

Here's the syntax of the command:

```
bzegrep [OPTIONS] PATTERN [FILE...]
```

- "OPTIONS": There are several options available that can modify the behavior of "bzegrep". These include "-c" (print only a count of matching lines), "-i" (ignore case), and "-v" (invert the match).
- "PATTERN": This is the regular expression that we want to search for in the compressed files.
- "FILE": This is the path to one or more compressed files that we want to search. If no file is specified, "bzegrep" will read from standard input.

Here's an example of how to use "bzegrep":

```
bzegrep -i "hello world" file1.bz2 file2.bz2
```

This command will search for the pattern "hello world" (case-insensitive) in the files "file1.bz2" and "file2.bz2".

Overall, "bzegrep" is a powerful command for searching through bzip2-compressed files. It's particularly useful when dealing with large log files or archives that are too big to fit in memory. 

## tldr 
 
> Find extended regular expression patterns in bzip2 compressed files using egrep.
> More information: <https://manned.org/bzegrep>.

- Search for extended regular expressions (supporting `?`, `+`, `{}`, `()` and `|`) in a compressed file (case-sensitive):

`bzegrep "{{search_pattern}}" {{path/to/file}}`

- Search for extended regular expressions (supporting `?`, `+`, `{}`, `()` and `|`) in a compressed file (case-insensitive):

`bzegrep --ignore-case "{{search_pattern}}" {{path/to/file}}`

- Search for lines that do not match a pattern:

`bzegrep --invert-match "{{search_pattern}}" {{path/to/file}}`

- Print file name and line number for each match:

`bzegrep --with-filename --line-number "{{search_pattern}}" {{path/to/file}}`

- Search for lines matching a pattern, printing only the matched text:

`bzegrep --only-matching "{{search_pattern}}" {{path/to/file}}`

- Recursively search files in a bzip2 compressed tar archive for a pattern:

`bzegrep --recursive "{{search_pattern}}" {{path/to/file}}`
