# zstd 
## chatgpt 
zstd is a compression utility that is used to compress and decompress files. It is a command line tool that offers high compression speeds, while maintaining a good balance between compression ratio and speed. The zstd compression algorithm is designed to achieve high speed and high compression rates, making it an ideal choice for use on large data sets.

To use the zstd command, you must first install it on your system. Once installed, you can open a terminal window on your system and use the following format to run the zstd command:

zstd [options] [input_file]

In this command, [options] are the various options and flags that you can use with the zstd command, and [input_file] is the file that you want to compress or decompress.

Some of the common options and flags that you can use with the zstd command include:

- -d : Use this flag to decompress a file that has been compressed with zstd.
- -f : Use this flag to force zstd to overwrite an existing output file.
- -k : Use this flag to keep the input file unmodified and create a compressed copy with a .zst extension.
- -v : Use this flag to show verbose output during compression or decompression.

To compress a file using zstd, simply provide the name of the file as the [input_file] parameter and zstd will compress the file and save it with a .zst extension. For example:

zstd myfile.txt

This command will compress the file "myfile.txt" and save it as "myfile.txt.zst".

To decompress a file that has been compressed with zstd, provide the -d flag followed by the name of the compressed file as the [input_file] parameter. For example:

zstd -d myfile.txt.zst

This command will decompress the file "myfile.txt.zst" and save it as "myfile.txt". 

## tldr 
 
> Compress or decompress files with Zstandard compression.
> More information: <https://github.com/facebook/zstd>.

- Compress a file into a new file with the `.zst` suffix:

`zstd {{path/to/file}}`

- Decompress a file:

`zstd -d {{path/to/file}}.zst`

- Decompress to `stdout`:

`zstd -dc {{path/to/file}}.zst`

- Compress a file specifying the compression level, where 1=fastest, 19=slowest and 3=default:

`zstd -{{level}} {{path/to/file}}`

- Unlock higher compression levels (up to 22) using more memory (both for compression and decompression):

`zstd --ultra -{{level}} {{path/to/file}}`
