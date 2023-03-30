# paste 
## chatgpt 
The `paste` command is a Linux/Unix utility that is used to join multiple files horizontally. It is typically used to merge the content of two or more text files line by line. Here is the syntax for the `paste` command:

```
paste [OPTION]... [FILE]...
```

The `[OPTION]...` parameter is optional and can be used to modify the behavior of the `paste` command. Here are some common options:

- `-d DELIM`: Specifies the delimiter that should be used to separate the merged lines. By default, the delimiter is a tab character.
- `-s`: Treats all input files as a single file, merging lines sequentially instead of horizontally.
- `-z`: Treats lines in the input files as null-terminated, instead of being terminated by a newline character.

The `[FILE]...` parameter represents the names of the files that you want to merge. You can specify multiple files, but at least one file must be provided. If you don't specify any files, the `paste` command will read from standard input.

Once you have specified the options and file names, the `paste` command will merge the files horizontally by appending the lines of the files together side-by-side. The output will be written to the standard output stream, which can be redirected to a file or piped to another command. 

## tldr 
 
> Merge lines of files.
> More information: <https://www.gnu.org/software/coreutils/paste>.

- Join all the lines into a single line, using TAB as delimiter:

`paste -s {{path/to/file}}`

- Join all the lines into a single line, using the specified delimiter:

`paste -s -d {{delimiter}} {{path/to/file}}`

- Merge two files side by side, each in its column, using TAB as delimiter:

`paste {{file1}} {{file2}}`

- Merge two files side by side, each in its column, using the specified delimiter:

`paste -d {{delimiter}} {{file1}} {{file2}}`

- Merge two files, with lines added alternatively:

`paste -d '\n' {{file1}} {{file2}}`
