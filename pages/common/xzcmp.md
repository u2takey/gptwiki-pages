# xzcmp 
## chatgpt 
The `xzcmp` command is used to compare or check the integrity of one or more compressed XZ files. The XZ format is a lossless data compression format that uses a combination of the LZMA2 compression algorithm and the delta encoding algorithm.

The syntax of the `xzcmp` command is as follows:

```
xzcmp [OPTION]... [FILE]...
```

Here, `OPTION` refers to any optional command-line arguments that can be provided with the command, and `FILE` refers to the file or files that need to be compared.

Some common options that can be used with the `xzcmp` command are:

- `-v, --verbose`: This option displays additional information about the files being compared, such as their sizes and compression ratios.
- `-q, --quiet`: This option suppresses all output from the command except for error messages.
- `-e, --error`: This option instructs the command to exit with an error status if any of the files being compared are not the same.

To use the `xzcmp` command, you simply need to provide the name or names of the XZ files that you want to compare as arguments. For example, to compare two files named `file1.xz` and `file2.xz`, you can run the following command:

```
xzcmp file1.xz file2.xz
```

The `xzcmp` command will then compare the contents of the two files and report whether they are the same or different. If there are any errors or discrepancies between the files, the command will display an error message to notify you. 

## tldr 
 
> Compare compressed files.
> More information: <https://manned.org/xzcmp>.

- Compare two specific files:

`xzcmp {{path/to/file1}} {{path/to/file2}}`
