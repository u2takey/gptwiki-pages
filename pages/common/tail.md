# tail 
## chatgpt 
`tail` is a command-line utility for displaying the end of a file. It reads the specified file and outputs the last few lines, which can be useful for monitoring log files, updating data in real-time, or debugging programs. 

The syntax of the `tail` command is:

```
tail [OPTIONS] [FILE]
```

Here, OPTIONS are the various flags and arguments that can be passed to the `tail` command to change its behavior, and FILE is the path to the file that you want to read.

Some commonly used options for `tail` are:

- `-n [N]`: displays the last N lines of the file. If N is not specified, it defaults to 10.
- `-f`: "follows" the file and displays new content as it is written to the file. Useful for monitoring log files in real time.
- `-q`: suppresses the header that displays the file name.
- `-s [SECONDS]`: specifies the number of seconds to sleep between updates when using the `-f` option.
- `-c [BYTES]`: displays the last N bytes of the file instead of lines.

For example, to display the last 20 lines of the file `log.txt`, you can use the command:

```
tail -n 20 log.txt
```

This will output the last 20 lines of the file `log.txt`.

Likewise, to continuously follow and display the updates to the same file, you can use the command:

```
tail -f log.txt
```

This will show any new content appended to the file `log.txt` as it appears in real time. 

## tldr 
 
> Display the last part of a file.
> See also: `head`.
> More information: <https://www.gnu.org/software/coreutils/tail>.

- Show last 'count' lines in file:

`tail --lines {{count}} {{path/to/file}}`

- Print a file from a specific line number:

`tail --lines +{{count}} {{path/to/file}}`

- Print a specific count of bytes from the end of a given file:

`tail --bytes {{count}} {{path/to/file}}`

- Print the last lines of a given file and keep reading file until `Ctrl + C`:

`tail --follow {{path/to/file}}`

- Keep reading file until `Ctrl + C`, even if the file is inaccessible:

`tail --retry --follow {{path/to/file}}`

- Show last 'num' lines in 'file' and refresh every 'n' seconds:

`tail --lines {{count}} --sleep-interval {{seconds}} --follow {{path/to/file}}`
