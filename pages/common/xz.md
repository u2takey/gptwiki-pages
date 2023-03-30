# xz 
## chatgpt 
xz is a command-line utility for compressing and decompressing files. 

The basic syntax of the command is: 

```xz [options] [file]```

Options:

Some common options used with xz command are:

- -z: to create a compressed archive file using xz
- -d: to decompress the archived file
- -k: to keep the original file when compressing or decompressing
- -v: to display the progress of the operation in the terminal
- -c: to print the output of xz to standard output (stdout) rather than a file

For example, to create a compressed archive file named `example.tar.xz` of a directory named `example`, the command would be:

```tar -cvf - example/ | xz -9 -c > example.tar.xz```

This command creates a tar archive of the `example` directory using `tar`, then pipes it to `xz` with the `-9` option, which indicates the highest level of compression. Finally, the output is redirected to a file named `example.tar.xz`. 

To decompress this archive, the command would be:

```xz -d example.tar.xz```

This would decompress the archive and create a directory named `example` in the current working directory. 

Overall, xz is a powerful command-line utility for compressing and decompressing files, and understanding its basic syntax and options can be useful for managing files and saving disk space. 

## tldr 
 
> Compress or decompress .xz and .lzma files.
> More information: <https://tukaani.org/xz/format.html>.

- Compress a file to the xz file format:

`xz {{path/to/file}}`

- Decompress a xz file:

`xz -d {{file.xz}}`

- Compress a file to the LZMA file format:

`xz --format={{lzma}} {{path/to/file}}`

- Decompress an LZMA file:

`xz -d --format={{lzma}} {{file.lzma}}`

- Decompress a file and write to `stdout`:

`xz -dc {{file.xz}}`

- Compress a file, but don't delete the original:

`xz -k {{path/to/file}}`

- Compress a file using the fastest compression:

`xz -0 {{path/to/file}}`

- Compress a file using the best compression:

`xz -9 {{path/to/file}}`
