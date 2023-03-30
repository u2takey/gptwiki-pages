# 7zr 
## chatgpt 
7zr is a command-line tool which is a part of the 7-Zip file archiver package. It is used for compressing and decompressing files with the 7z file format.

The "7" in "7z" stands for seven layers of compression - it is a high compression ratio format that can compress files into a smaller size. "z" represents the format type of the resulting compressed file.

The "r" flag in "7zr" stands for "read", which allows the compressed file to be read and extracted without writing it back to disk. 

When using the "7zr" command, you can specify various options to customize the compression settings, such as compression level, file format, and password protection. 

To compress files using 7zr, enter the following command in the terminal: 

```bash
7zr a [archive name] [file or directory to be compressed]
```

To extract compressed files, enter the following command:

```bash
7zr x [compressed file name]
```

Overall, 7zr is a powerful command-line tool used for compressing and decompressing files in a highly efficient manner, and can be used as a alternative to other compression software packages. 

## tldr 
 
> File archiver with a high compression ratio.
> Similar to `7z` except that it only supports `.7z` files.
> More information: <https://www.7-zip.org>.

- [a]rchive a file or directory:

`7zr a {{path/to/archive.7z}} {{path/to/file_or_directory}}`

- Encrypt an existing archive (including file names):

`7zr a {{path/to/encrypted.7z}} -p{{password}} -mhe=on {{path/to/archive.7z}}`

- E[x]tract an archive preserving the original directory structure:

`7zr x {{path/to/archive.7z}}`

- E[x]tract an archive to a specific directory:

`7zr x {{path/to/archive.7z}} -o{{path/to/output}}`

- E[x]tract an archive to `stdout`:

`7zr x {{path/to/archive.7z}} -so`

- [l]ist the contents of an archive:

`7zr l {{path/to/archive.7z}}`

- List available archive types:

`7zr i`
