# gzip 
## chatgpt 
The command `gzip` is used to compress files in Unix and Unix-like operating systems. The basic syntax of the command is:

`gzip [options] [file(s)]`

The `options` can be used to specify additional features and behaviors of the command, while the `file(s)` are the filenames of the files that should be compressed or decompressed.

The most commonly used options of the `gzip` command include:

- `-d` or `--decompress`: This specifies that the command should decompress (i.e., uncompress) the specified file.
- `-f` or `--force`: This specifies that the command should force the compression or decompression, even if it would overwrite an existing file.
- `-r` or `--recursive`: This specifies that the command should recursively compress or decompress all files in a directory and its subdirectories.
- `-v` or `--verbose`: This specifies that the command should display verbose output during the compression or decompression process.

The `gzip` command creates a compressed file with a `.gz` file extension by default when compressing a file. When decompressing a file, the `.gz` extension is removed from the resulting decompressed file.

Some examples of using the `gzip` command include:

- Compressing a file: `gzip myfile.txt` This will compress the file `myfile.txt` and create a new file `myfile.txt.gz`.
- Decompressing a file: `gzip -d myfile.txt.gz` This will decompress the file `myfile.txt.gz` and create a new file `myfile.txt`.
- Compressing all files in a directory: `gzip -r /path/to/directory/` This will compress all files in the directory and its subdirectories, retaining the original file names and adding the `.gz` extension to the compressed files. 

## tldr 
 
> Compress/uncompress files with gzip compression (LZ77).
> More information: <https://www.gnu.org/software/gzip/manual/gzip.html>.

- Compress a file, replacing it with a gzipped compressed version:

`gzip {{file.ext}}`

- Decompress a file, replacing it with the original uncompressed version:

`gzip -d {{file.ext}}.gz`

- Compress a file, keeping the original file:

`gzip --keep {{file.ext}}`

- Compress a file specifying the output filename:

`gzip -c {{file.ext}} > {{compressed_file.ext.gz}}`

- Decompress a gzipped file specifying the output filename:

`gzip -c -d {{file.ext}}.gz > {{uncompressed_file.ext}}`

- Specify the compression level. 1=Fastest (Worst), 9=Slowest (Best), Default level is 6:

`gzip -9 -c {{file.ext}} > {{compressed_file.ext.gz}}`
