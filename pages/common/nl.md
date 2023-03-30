# nl 
## chatgpt 
The `nl` command is a Unix and Linux command used to number lines in a file. The name "nl" is short for "number lines". The basic syntax of the command is:

```
nl [options] [file]
```

Here, `options` are the flags that modify the operation of the command, and `file` is the name of the file to be numbered.

Some commonly used options of the `nl` command are:

- `-b` specifies the type of numbering to use. It can take three values:
    - `a`: Number all lines
    - `t`: Number only non-empty lines
    - `n`: Do not number any lines
- `-w` sets the width of the line number field. By default, it is set to 6.
- `-s` specifies the string to use as a line number separator. By default, it is set to a tab character.

For example, to number all lines in a file called `example.txt` starting from 1 and with a line number width of 3, you could use the command:

```
nl -b a -w 3 example.txt
```

This would output the contents of `example.txt`, with each line preceded by its line number, padded with zeros if necessary to make it three digits wide. 

## tldr 
 
> A utility for numbering lines, either from a file, or from standard input.
> More information: <https://www.gnu.org/software/coreutils/nl>.

- Number non-blank lines in a file:

`nl {{path/to/file}}`

- Read from standard output:

`cat {{path/to/file}} | nl {{options}} -`

- Number only the lines with printable text:

`nl -t {{path/to/file}}`

- Number all lines including blank lines:

`nl -b a {{path/to/file}}`

- Number only the body lines that match a basic regular expression (BRE) pattern:

`nl -b p'FooBar[0-9]' {{path/to/file}}`
