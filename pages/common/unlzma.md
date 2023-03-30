# unlzma 
## chatgpt 
The `unlzma` command is used to decompress LZMA-compressed files. LZMA is a data compression algorithm developed by Russian programmer Igor Pavlov. It provides high compression ratio and fast decompression.

The `unlzma` command, sometimes written as `lzma -d`, is usually used in Linux and Unix systems to decompress LZMA-compressed files. It takes one or more files as arguments and decompresses them, creating an uncompressed version of the file with the same name, but without the ".lzma" extension.

Some common options that can be used with the `unlzma` command are:

- `-c`, which writes the decompressed file to standard output instead of a file
- `-f`, which forces overwriting of an existing file
- `-k`, which keeps the original compressed file after decompression

For example, to decompress a file named `file.lzma` and create an uncompressed version of it, the `unlzma` command can be used like this:

```
unlzma file.lzma
```

This will create a new file named `file` in the same directory, with the uncompressed data from the original compressed file. 

## tldr 
 
> This command is an alias of `xz --format=lzma --decompress`.
> More information: <https://manned.org/unlzma>.

- View documentation for the original command:

`tldr xz`
