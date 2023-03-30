# fgrep 
## chatgpt 
fgrep (or "fixed-string grep") is a command-line utility used to search for a specific string or text pattern in one or more files. It is a variant of the grep command, but it treats the search string as a fixed, literal string instead of a regular expression. This means that it will only search for the exact same string that is entered as an argument, without any special characters or patterns.

The syntax for using fgrep is as follows:

```
fgrep [options] pattern [file(s)]
```

- options: These are optional flags that can modify the behavior of the fgrep command, such as -i (case-insensitive search) or -r (recursive search).
- pattern: This is the fixed string or text pattern that fgrep will search for in the specified file(s).
- file(s): These are the name(s) of the file(s) that fgrep will search in. If no file is specified, the standard input (stdin) will be used.

For example, to search for the string "apple" in the file "fruits.txt", you can use the following command:

```
fgrep apple fruits.txt
```

This will return all lines in the file "fruits.txt" that contain the exact string "apple".

Note that fgrep is a deprecated command and has been replaced by the equivalent "grep -F" command. 

## tldr 
 
> Matches fixed strings in files.
> Equivalent to `grep -F`.
> More information: <https://www.gnu.org/software/grep/manual/grep.html>.

- Search for an exact string in a file:

`fgrep {{search_string}} {{path/to/file}}`

- Search only lines that match entirely in files:

`fgrep -x {{path/to/file1}} {{path/to/file2}}`

- Count the number of lines that match the given string in a file:

`fgrep -c {{search_string}} {{path/to/file}}`

- Show the line number in the file along with the line matched:

`fgrep -n {{search_string}} {{path/to/file}}`

- Display all lines except those that contain the search string:

`fgrep -v {{search_string}} {{path/to/file}}`

- Display filenames whose content matches the search string at least once:

`fgrep -l {{search_string}} {{path/to/file1}} {{path/to/file2}}`
