# grep 
## chatgpt 
grep is a Unix/Linux command that stands for "Global Regular Expression Print". It is used for searching for a specific pattern or regular expression in a file(s) or output of a command.

The syntax for using grep is as follows:

```
grep [options] pattern [file or directory]
```

- options: These are optional parameters that modify the behavior of the grep command. Some commonly used options are:
  - -i: Ignore case while searching
  - -v: Invert the match (i.e. print lines that do not match the pattern)
  - -n: Print the line numbers along with the matched lines
  - -r: Search recursively in subdirectories
  - -e: Use a regular expression as the search pattern
- pattern: This is the regular expression or search string that grep uses to find matches.
- file or directory: This is the file(s) or directory in which grep should search for the pattern. If no file or directory is specified, grep reads from the standard input (stdin).

Here are some examples of using grep:

```
grep "hello" myfile.txt         # search for the word "hello" in the file myfile.txt
grep -i "HELLO" myfile.txt      # search for the word "hello" case-insensitively in the file myfile.txt
grep -rn "error" /var/log      # search for the word "error" recursively in the directory /var/log and print the line numbers
ps aux | grep "chrome"          # search for the process that contains the word "chrome"
```

Overall, grep is a powerful command for searching and filtering text data in Unix/Linux systems. 

## tldr 
 
> Find patterns in files using regular expressions.
> More information: <https://www.gnu.org/software/grep/manual/grep.html>.

- Search for a pattern within a file:

`grep "{{search_pattern}}" {{path/to/file}}`

- Search for an exact string (disables regular expressions):

`grep --fixed-strings "{{exact_string}}" {{path/to/file}}`

- Search for a pattern in all files recursively in a directory, showing line numbers of matches, ignoring binary files:

`grep --recursive --line-number --binary-files={{without-match}} "{{search_pattern}}" {{path/to/directory}}`

- Use extended regular expressions (supports `?`, `+`, `{}`, `()` and `|`), in case-insensitive mode:

`grep --extended-regexp --ignore-case "{{search_pattern}}" {{path/to/file}}`

- Print 3 lines of context around, before, or after each match:

`grep --{{context|before-context|after-context}}={{3}} "{{search_pattern}}" {{path/to/file}}`

- Print file name and line number for each match with color output:

`grep --with-filename --line-number --color=always "{{search_pattern}}" {{path/to/file}}`

- Search for lines matching a pattern, printing only the matched text:

`grep --only-matching "{{search_pattern}}" {{path/to/file}}`

- Search `stdin` for lines that do not match a pattern:

`cat {{path/to/file}} | grep --invert-match "{{search_pattern}}"`
