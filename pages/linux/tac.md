# tac 
## chatgpt 
The `tac` command is a Unix/Linux utility that is used to reverse the order of lines in a file. The `tac` command is the reverse of the `cat` command, which outputs the contents of a file from the first line to the last line. Here is an example of how to use the `tac` command:

```
tac filename
```

where `filename` is the name of the file you want to reverse. The `tac` command reads the file from the last line to the first line and writes the lines to the standard output in reverse order. 

For example, consider the following file:

```
$ cat file.txt
Line 1
Line 2
Line 3
```

If you use the `tac` command on this file, then the output will be:

```
$ tac file.txt
Line 3
Line 2
Line 1
```

This command is useful when you want to see the lines of a file in reverse order, or if you want to search for a pattern in a file starting from the end of the file to the beginning. 

## tldr 
 
> Display and concatenate files with lines in reversed order.
> See also: `cat`.
> More information: <https://www.gnu.org/software/coreutils/tac>.

- Concatenate specific files in reversed order:

`tac {{path/to/file1 path/to/file2 ...}}`

- Display `stdin` in reversed order:

`{{cat path/to/file}} | tac`

- Use a specific separator:

`tac --separator {{,}} {{path/to/file1 path/to/file2 ...}}`

- Use a specific regex as a separator:

`tac --regex --separator {{[,;]}} {{path/to/file1 path/to/file2 ...}}`

- Use a separator before each file:

`tac --before {{path/to/file1 path/to/file2 ...}}`
