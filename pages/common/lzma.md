# lzma 
## chatgpt 
The `lzma` command is a Linux utility used for compressing and decompressing files using the LZMA compression algorithm. LZMA (Lempel–Ziv–Markov chain algorithm) is a lossless data compression algorithm that uses a combination of dictionary compression techniques and statistical modeling to achieve high compression ratios.

When using the `lzma` command to compress a file, the syntax is as follows:

```
lzma [OPTIONS] FILE
```

Here, `[OPTIONS]` refers to any additional command line options you want to specify, and `FILE` refers to the name of the file you want to compress.

Some commonly used options with the `lzma` command include:

- `-d` or `--decompress`: decompresses the specified file instead of compressing it.
- `-k` or `--keep`: preserves the original file when compressing or decompressing, creating a new file with the ".lzma" extension.
- `-v` or `--verbose`: displays verbose output, showing statistics about the compression or decompression process.

For example, to compress a file called `myfile.txt` using the `lzma` command with maximum compression, you would run the following command:

```
lzma -9 myfile.txt
```

This would create a compressed file called `myfile.txt.lzma` in the same directory as the original file. To decompress the file, you would run the `lzma` command with the `-d` option:

```
lzma -d myfile.txt.lzma
```

This would decompress the `myfile.txt.lzma` file and create a new file called `myfile.txt` in the same directory. 

## tldr 
 
> This command is an alias of `xz --format=lzma`.
> More information: <https://manned.org/lzma>.

- View documentation for the original command:

`tldr xz`
