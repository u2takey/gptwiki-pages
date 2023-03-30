# hexdump 
## chatgpt 
hexdump is a command used in Unix and Linux operating systems to display the contents of a binary file in hexadecimal format. This command is used to display the hexadecimal representation of the content of a file in the standard output. 

When you run the command 'hexdump' followed by the name of the file as an argument, it opens the file for reading and displays the hexadecimal representation of its contents. By default, hexdump shows 16 bytes per row with their respective hexadecimal values, ASCII characters, and printable character translations. It displays a series of hexadecimal numbers that represent the contents of the file. 

This command can be helpful in analyzing and debugging binary files or when you need to examine the actual data of a file. It can be used to view any type of binary file, including executable files, object files, libraries, and firmware.

There are several options that can be used with the hexdump command to modify its behavior. For example, you can use the 'C' option to display only the ASCII characters corresponding to the hexadecimal code, 'n' to specify the number of bytes to be displayed, and 's' to specify the starting offset from where dump the data. 

Overall, the hexdump command is useful to examine binary files and analyze their contents in a readable and organized format. 

## tldr 
 
> An ASCII, decimal, hexadecimal, octal dump.
> More information: <https://manned.org/hexdump>.

- Print the hexadecimal representation of a file, replacing duplicate lines by '*':

`hexdump {{path/to/file}}`

- Display the input offset in hexadecimal and its ASCII representation in two columns:

`hexdump -C {{path/to/file}}`

- Display the hexadecimal representation of a file, but interpret only n bytes of the input:

`hexdump -C -n{{number_of_bytes}} {{path/to/file}}`

- Don't replace duplicate lines with '*':

`hexdump --no-squeezing {{path/to/file}}`
