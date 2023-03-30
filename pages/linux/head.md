# head 
## chatgpt 
The `head` command is a Unix/Linux command that is used to display the first few lines of a file on the terminal screen. By default, it displays the first 10 lines of a file.

The syntax of the `head` command is as follows:

```
head [OPTION]... [FILE]...
```

Here, `[OPTION]` and `[FILE]` are optional parameters that can be used with the `head` command. 

Some commonly used options with the `head` command are:

- `-n` or `--lines`: This option is used to specify the number of lines to be displayed. For example, `head -n 5 file.txt` will display the first 5 lines of the file `file.txt`.
- `-c` or `--bytes`: This option is used to specify the number of bytes to be displayed. For example, `head -c 20 file.txt` will display the first 20 bytes of the file `file.txt`.
- `-q` or `--quiet`: This option is used to suppress the display of header information.
- `-v` or `--verbose`: This option is used to display the header information.

If you don't specify any option or file name with the `head` command, it will display the first 10 lines of the standard input.

For example, `head file.txt` will display the first 10 lines of `file.txt` on the terminal screen. 

## tldr 
 
> Output the first part of files.
> More information: <https://www.gnu.org/software/coreutils/head>.

- Output the first few lines of a file:

`head --lines {{count}} {{path/to/file}}`

- Output the first few bytes of a file:

`head --bytes {{count}} {{path/to/file}}`

- Output everything but the last few lines of a file:

`head --lines -{{count}} {{path/to/file}}`

- Output everything but the last few bytes of a file:

`head --bytes -{{count}} {{path/to/file}}`
