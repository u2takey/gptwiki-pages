# p7zip 
## chatgpt 
p7zip is a command-line file archiver with a high compression ratio that is primarily used for compressing and decompressing files. It is an open-source alternative to the popular file archiving tools like WinZip and WinRAR.

The p7zip command is used to create, manipulate, and extract files from the 7z archive format. It supports a range of compression algorithms like LZMA, LZMA2, PPMD, Bzip2, and others.

To use the p7zip command, you need to open a terminal window and enter the command with the desired options and arguments. Here are some examples of how to use the p7zip command:

1. To compress a file or directory:

```
7z a archive.7z file.txt
```

This command will create a compressed archive named archive.7z that contains the file.txt file. You can replace file.txt with the name of a directory to compress its contents.

2. To extract files from an archive:

```
7z x archive.7z
```

This command will extract all the files from the archive named archive.7z to the current directory.

3. To list the contents of an archive:

```
7z l archive.7z
```

This command will list all the files and folders contained in the archive named archive.7z.

There are many other options available in the p7zip command that can be used to customize the compression and extraction process, such as password protection, splitting archives into multiple parts, and more. You can check the p7zip manual for more information. 

## tldr 
 
> Wrapper of 7-Zip file archiver with high compression ratio.
> Internally executes either 7za or 7zr command.
> More information: <http://p7zip.sourceforge.net>.

- Archive a file, replacing it with a 7zipped compressed version:

`p7zip {{path/to/file}}`

- Archive a file keeping the input file:

`p7zip -k {{path/to/file}}`

- Decompress a file, replacing it with the original uncompressed version:

`p7zip -d {{compressed.ext}}.7z`

- Decompress a file keeping the input file:

`p7zip -d -k {{compressed.ext}}.7z`

- Skip some checks and force compression or decompression:

`p7zip -f {{path/to/file}}`
