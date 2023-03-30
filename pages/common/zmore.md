# zmore 
## chatgpt 
Zmore is a command used in UNIX or Linux operating systems. It is used to display the contents of a compressed file in the terminal. Specifically, zmore is used to display contents of text files compressed using the "compress" utility that comes with UNIX systems.

When you enter the "zmore" command in the terminal, it opens the specified compressed file and displays the contents of the file one screen at a time, allowing the user to scroll through the file using the spacebar or arrow keys. The zmore command is similar to the "more" command, which is used to display text files that are not compressed.

The zmore command can be useful when you need to view the contents of a compressed file but do not want to extract or decompress the file. It saves disk space and time as you don't need to extract the file before reading it.

In summary, the zmore command displays compressed files without extracting them, allowing you to conveniently view the contents of the file in a terminal window. 

## tldr 
 
> View gzip compressed files with `more`.
> More information: <https://manned.org/zmore>.

- Open a compressed file:

`zmore {{path/to/file.txt.gz}}`

- Display the next page of the file:

`<Space>`

- Search for a pattern in the file (press `n` to go to next match):

`/{{regular_expression}}`

- Exit:

`q`

- Display interactive command help:

`h`
