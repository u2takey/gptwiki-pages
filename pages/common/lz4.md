# lz4 
## chatgpt 
lz4 is a command line utility that is used for data compression and decompression. It is a fast and lightweight compression tool that was designed to provide high compression and decompression speeds.

The lz4 command compresses input files or streams into output files or streams, depending on the user's requirement. This compression algorithm is highly optimized for speed and efficiency, making it an ideal option for real-time applications and situations where data is being processed on the fly.

The lz4 command has various parameters and options that enable users to fine-tune the compression process according to their needs. Some of the most commonly used options include:

- -c: Compress the input file and send the output to the standard output stream.

- -d: Decompress the input file and send the output to the standard output stream.

- -f: Force overwriting of existing output files.

- -k: Keep the input file despite compression or decompression.

- -z: Compress with the gzip format.

- -v: Verbose mode. Displays the compression/decompression progress.

Overall, the lz4 command offers a highly efficient and fast compression algorithm that can be used in a wide range of applications to save disk space, reduce network traffic, and speed up data processing. 

## tldr 
 
> Compress or decompress .lz4 files.
> More information: <https://github.com/lz4/lz4>.

- Compress a file:

`lz4 {{path/to/file}}`

- Decompress a file:

`lz4 -d {{file.lz4}}`

- Decompress a file and write to `stdout`:

`lz4 -dc {{file.lz4}}`

- Package and compress a directory and its contents:

`tar cvf - {{path/to/directory}} | lz4 - {{dir.tar.lz4}}`

- Decompress and unpack a directory and its contents:

`lz4 -dc {{dir.tar.lz4}} | tar -xv`

- Compress a file using the best compression:

`lz4 -9 {{path/to/file}}`
