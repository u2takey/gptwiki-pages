# lzip 
## chatgpt 
lzip is a command-line program that is used to compress or decompress files using the LZMA algorithm. The LZMA algorithm is a compression algorithm that provides very high compression ratios and can handle extremely large files.

The basic syntax of the lzip command is:

lzip [options] file

Here, 'file' is the name of the file that needs to be compressed or decompressed. The 'options' parameter is optional and can be used to set various options for the lzip command.

Some of the commonly used options with the lzip command are:

- -d: This option is used to decompress a file that has been compressed using the lzip command.
- -c: This option is used to output the compressed data to the standard output instead of a file.
- -v: This option is used to display verbose output while compressing or decompressing a file.
- -k: This option is used to keep the original file after compressing or decompressing it.
- -f: This option is used to force compression or decompression of a file, even if it already exists.

Overall, the lzip command is a powerful tool for compressing and decompressing large files using the LZMA algorithm, and can be used effectively in a variety of applications. 

## tldr 
 
> Lzip is a lossless data compressor with a user interface similar to `gzip` or `bzip2`.
> Lzip uses a simplified form of the "Lempel-Ziv-Markovchain-Algorithm"z (LZMA) stream format and provides a 3 factor integrity checking to maximize interoperability and optimize safety.
> More information: <https://www.nongnu.org/lzip>.

- Archive a file, replacing it with with a compressed version:

`lzip {{path/to/file}}`

- Archive a file, keeping the input file:

`lzip -k {{path/to/file}}`

- Archive a file with the best compression (level=9):

`lzip -k {{path/to/file}} --best`

- Archive a file at the fastest speed (level=0):

`lzip -k {{path/to/file}} --fast`

- Test the integrity of compressed file:

`lzip --test {{path/to/archive.lz}}`

- Decompress a file, replacing it with the original uncompressed version:

`lzip -d {{path/to/archive.lz}}`

- Decompress a file, keeping the archive:

`lzip -d -k {{path/to/archive.lz}}`

- List files which are in an archive and show compression stats:

`lzip --list {{path/to/archive.lz}}`
