# pigz 
## chatgpt 
pigz is a command-line utility program used to compress or decompress files. 

When used to compress files, pigz creates compressed files from input files using the gzip algorithm. It supports parallel compression of input files using multiple processors, making the compression process faster. 

The command syntax for pigz is as follows:

```
pigz [options] [file(s)]
```

Some common options include:

- `-k`: keep input file(s), i.e., do not delete the original file(s)
- `-p`: set the number of processors to use for parallel compression (default is the number of available processors)
- `-c`: write the compressed output to standard output instead of creating a compressed file
- `-d`: decompress input file(s)
- `-r`: compress a directory and its contents recursively

Examples:

1. Compress a single file using pigz:

```
pigz file.txt
```

This will create a compressed file `file.txt.gz` in the same directory as the original `file.txt`, and delete the original file.

2. Compress multiple files using pigz:

```
pigz file1.txt file2.txt file3.txt
```

This will create compressed files `file1.txt.gz`, `file2.txt.gz`, and `file3.txt.gz` in the same directory where the original files are located.

3. Compress a directory and its contents using pigz:

```
pigz -r directory/
```

This will recursively compress all files in the directory and its subdirectories, creating the compressed files with the `.gz` extension. 

4. Decompress a single file using pigz:

```
pigz -d file.txt.gz
```

This will decompress the compressed file `file.txt.gz` and create the uncompressed file `file.txt` in the same directory. 

## tldr 
 
> Multithreaded zlib compression utility.
> More information: <https://github.com/madler/pigz>.

- Compress a file with default options:

`pigz {{path/to/file}}`

- Compress a file using the best compression method:

`pigz -9 {{path/to/file}}`

- Compress a file using no compression and 4 processors:

`pigz -0 -p{{4}} {{path/to/file}}`

- Compress a directory using tar:

`tar cf - {{path/to/directory}} | pigz > {{path/to/file}}.tar.gz`

- Decompress a file:

`pigz -d {{archive.gz}}`

- List the contents of an archive:

`pigz -l {{archive.tar.gz}}`
