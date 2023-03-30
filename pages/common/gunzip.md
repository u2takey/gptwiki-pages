# gunzip 
## chatgpt 
The `gunzip` command is a UNIX/Linux utility used for decompressing files that have been compressed using the `gzip` compression algorithm. This command is primarily used to extract files that have the ".gz" file extension. 

The basic syntax of the `gunzip` command is as follows:

```
gunzip [OPTIONS] [FILE-NAME(s)]
```

Here, the `OPTIONS` are used to specify optional parameters for the command. The `FILE-NAME(s)` are the names of the files that need to be decompressed. 

Some of the commonly used options for the `gunzip` command are:

- `-c` - Write output to standard output instead of overwriting the input file(s).
- `-f` - Force operation to ignore non-fatal errors and overwrite existing output files.
- `-k` - Keep the input file(s) after compression. By default, the input file(s) are deleted.
- `-r` - Recursively decompress files in directories and subdirectories.

For example, to decompress a file named "example.gz" using `gunzip`, you can use the following command:

```
gunzip example.gz
```

This will decompress the file and create a new file named "example" in the same directory.

Alternatively, if you want to keep the original file intact and write the output to standard output, you can use the following command:

```
gunzip -c example.gz
```

This will decompress the file and print the output to the console without overwriting the input file. 

## tldr 
 
> Extract file(s) from a gzip (.gz) archive.
> More information: <https://manned.org/gunzip>.

- Extract a file from an archive, replacing the original file if it exists:

`gunzip {{archive.tar.gz}}`

- Extract a file to a target destination:

`gunzip --stdout {{archive.tar.gz}} > {{archive.tar}}`

- Extract a file and keep the archive file:

`gunzip --keep {{archive.tar.gz}}`

- List the contents of a compressed file:

`gunzip --list {{file.txt.gz}}`

- Decompress an archive from `stdin`:

`cat {{path/to/archive.gz}} | gunzip`
