# bzip2 
## chatgpt 
bzip2 is a command-line compression utility that is used to compress and decompress files using the Burrows-Wheeler block sorting text compression algorithm and Huffman coding. 

The basic syntax for the bzip2 command is as follows:

```bash
bzip2 [OPTIONS] [FILE]
```

Some common options used with the bzip2 command are:

- `-d` or `--decompress`: This option is used to decompress bzip2-compressed files.
- `-k` or `--keep`: This option is used to keep the original file after compression and create a compressed copy with the .bz2 extension.
- `-c` or `--stdout`: This option is used to send the compressed output to standard output instead of creating a compressed file.
- `-v` or `--verbose`: This option is used to display verbose output while compressing or decompressing files.

For example, if you want to compress a file named `testfile.txt` using bzip2 and keep the original file, you can use the following command:

```bash
bzip2 -k testfile.txt
```

This will create a compressed file named `testfile.txt.bz2` while keeping the original file intact.

Similarly, if you want to decompress the compressed file `testfile.txt.bz2`, you can use the following command:

```bash
bzip2 -d testfile.txt.bz2
```

This will decompress the compressed file and create a file named `testfile.txt`. 

## tldr 
 
> A block-sorting file compressor.
> More information: <https://manned.org/bzip2>.

- Compress a file:

`bzip2 {{path/to/file_to_compress}}`

- Decompress a file:

`bzip2 -d {{path/to/compressed_file.bz2}}`

- Decompress a file to standard output:

`bzip2 -dc {{path/to/compressed_file.bz2}}`

- Test the integrity of each file inside the archive file:

`bzip2 --test {{path/to/compressed_file.bz2}}`

- Show the compression ratio for each file processed with detailed information:

`bzip2 --verbose {{path/to/compressed_files.bz2}}`

- Decompress a file overwriting existing files:

`bzip2 --force {{path/to/compressed_file.bz2}}`

- Display help:

`bzip2 -h`
