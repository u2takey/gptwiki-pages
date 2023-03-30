# hexyl 
## chatgpt 
Hexyl is a command-line tool for inspecting and visualizing binary data. It is used to display the hexadecimal (base 16) representation of binary data in a user-friendly way. The tool is designed to work with a variety of binary formats, including files, standard input, and process memory.

Once you have installed the hexyl tool on your system, you can run it by typing "hexyl" in the terminal. The default behavior of hexyl is to read from standard input and display the hexadecimal representation of the data.

You can also specify a file name as an argument to hexyl to view the hexadecimal representation of the file. For example, "hexyl myfile.bin" will display the data in the file myfile.bin in hexadecimal format.

Hexyl also provides a number of options to customize its output. For example, you can use the "-n" option to specify the number of bytes to display, or the "-c" option to specify the number of columns to use for the output.

One of the unique features of hexyl is its ability to display binary data in a variety of visual formats. By default, hexyl displays data in a traditional hexdump format. However, you can also use the "-f" option to display data as ASCII characters, or the "-b" option to display data as binary digits.

Overall, hexyl is a powerful tool for exploring binary data and can be used for a variety of tasks, including reverse engineering, malware analysis, and data forensics. 

## tldr 
 
> A simple hex viewer for the terminal. Uses colored output to distinguish different categories of bytes.
> More information: <https://github.com/sharkdp/hexyl>.

- Print the hexadecimal representation of a file:

`hexyl {{path/to/file}}`

- Print the hexadecimal representation of the first n bytes of a file:

`hexyl -n {{n}} {{path/to/file}}`

- Print bytes 512 through 1024 of a file:

`hexyl -r {{512}}:{{1024}} {{path/to/file}}`

- Print 512 bytes starting at the 1024th byte:

`hexyl -r {{1024}}:+{{512}} {{path/to/file}}`
