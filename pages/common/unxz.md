# unxz 
## chatgpt 
The "unxz" command is used in Linux and Unix operating systems to decompress or extract files that have been compressed with the XZ compression algorithm. 

The syntax of the "unxz" command is:

```
unxz [options] file.xz
```

Here, "file.xz" is the name of the compressed file that needs to be decompressed or extracted. 

Some common options used with the "unxz" command are:

- "-v" or "--verbose": This option makes the command output more information about the decompression process.
- "-d" or "--decompress": This option tells the command to just decompress the file without creating a new file. The original compressed file is replaced with the decompressed version.
- "-k" or "--keep": This option makes the command keep the original compressed file even after extracting its contents.
- "-c" or "--stdout": This option sends the decompressed output to the standard output (stdout) instead of creating a new file.

For example, to decompress a file named "file.xz" and keep the original file, the following command can be used:

```
unxz -k file.xz
```

This will create a new file named "file" containing the decompressed contents of "file.xz", while "file.xz" remains intact. 

## tldr 
 
> This command is an alias of `xz --decompress`.
> More information: <https://manned.org/unxz>.

- View documentation for the original command:

`tldr xz`
