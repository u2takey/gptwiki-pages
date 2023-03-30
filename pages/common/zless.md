# zless 
## chatgpt 
The 'zless' command is used to view the contents of a compressed file without having to decompress it first. 

When you use 'zless' followed by the name of a compressed file, the command directly opens the compressed file and displays its contents on the terminal. You can navigate through the file using the same commands as in 'less' command, such as scrolling up and down the file using the arrow keys, jumping to a specific line using the 'g' command, searching for text using the forward slash ("/") command, and quitting the file using the 'q' command.

The 'zless' command is particularly useful when you have a compressed file that is too large to easily decompress, or when there's not enough disk space available to hold both the uncompressed file and the original file. By using 'zless', you can quickly preview the contents of a compressed file without consuming much storage. 

## tldr 
 
> View `gzip` and `xz` compressed files.
> More information: <https://manned.org/zless>.

- Page through a `gzip` compressed file with `less`:

`zless {{file.txt.gz}}`
