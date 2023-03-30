# unzstd 
## chatgpt 
unzstd is a command used to decompress files that have been compressed using the zstandard algorithm. The zstandard algorithm is a lossless compression algorithm that provides good compression ratios and fast decompression times.

The syntax of the command is:

unzstd [options] [file]

Options:

- -c, --stdout: This option directs the output to the standard output instead of a file. This is useful when using the pipe command to send the compressed output to another command without creating an intermediate file.
- -d, --decompress: This option specifies that the input file should be decompressed. It is optional because unzstd can detect whether the input file is compressed or not.
- -f, --force: This option forces the output to be written even if it overwrites an existing file.
- -k, --keep: This option keeps the input file after it has been decompressed. By default, unzstd removes the input file after the output file is created.
- -q, --quiet: This option suppresses all warning messages.
- -t, --test: This option tests the integrity of the compressed file without decompressing it.
- -v, --verbose: This option prints extra information about the decompression process.

File:

The input file that needs to be decompressed. It can be any file compressed using the zstandard algorithm.

Example:

To decompress a file "sample.zst" and keep the original file, the following command can be used:

unzstd -k sample.zst

This will create a decompressed file "sample" while preserving the original compressed file. 

## tldr 
 
> Decompress files with Zstandard compression.
> More information: <https://github.com/facebook/zstd>.

- Decompress files:

`unzstd {{path/to/file1.ztd path/to/file2.ztd ...}}`

- Decompress a file into a specific output file:

`unzstd {{path/to/compressed.ztd}} -o {{path/to/extracted_file}}`

- Display information about a compressed file:

`unzip --list {{path/to/file.zst}}`
