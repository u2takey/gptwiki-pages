# more 
## chatgpt 
The `more` command is a command-line utility that is used to display the contents of a file one page at a time. This is particularly useful for long text files, where scrolling through the entire file would be impractical.

When you execute the `more` command, it defaults to displaying the contents of the specified file one page at a time. To move to the next page, you simply press the spacebar. Pressing the Enter key will display the next line of the file.

There are several options you can use with the `more` command to customize its behavior. For example, you can use the `-p` option to specify a pattern to search for in the file, and the `-c` option to colorize the output.

The `more` command is often used in conjunction with other commands in shell scripts to display the output of a command one page at a time. For example, you might use `ls | more` to display the contents of a directory one page at a time. 

## tldr 
 
> Display paginated output from `stdin` or a file.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/more>.

- Display paginated output from `stdin`:

`{{echo test}} | more`

- Display paginated output from one or more files:

`more {{path\to\file}}`

- Convert tabs to the specified number of spaces:

`more {{path\to\file}} /t{{spaces}}`

- Clear the screen before displaying the page:

`more {{path\to\file}} /c`

- Display the output starting at line 5:

`more {{path\to\file}} +{{5}}`

- Enable extended interactive mode (see help for usage):

`more {{path\to\file}} /e`

- Display full usage information:

`more /?`
