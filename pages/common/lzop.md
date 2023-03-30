# lzop 
## chatgpt 
lzop is a command-line utility used for compressing and decompressing files in Linux systems. It is used to compress large files to save disk space and to speed up data transfer.

To use the lzop command, you first need to install it on your Linux system. You can do this by using the following command:

```
sudo apt-get install lzop
```

Once installed, you can use the lzop command to compress a file using the following syntax:

```
lzop <filename>
```

For example, to compress a file named "file.txt", you would use the following command:

```
lzop file.txt
```

This will create a compressed file named "file.txt.lzo" in the same directory.

To decompress a compressed file using the lzop command, you can use the following syntax:

```
lzop -d <filename>
```

For example, to decompress a file named "file.txt.lzo", you would use the following command:

```
lzop -d file.txt.lzo
```

This will create a decompressed file named "file.txt" in the same directory.

lzop also has various options that you can use with the command. For example, the "-v" option can be used to display the compression ratio and the "-k" option can be used to keep the original file after compression. You can learn more about these options by using the following command:

```
lzop --help
``` 

## tldr 
 
> Compress or decompress files with LZO compression.
> More information: <https://www.lzop.org/>.

- Compress a file into a new file with the `.lzo` suffix:

`lzop {{path/to/file}}`

- Decompress a file:

`lzop -d {{path/to/file}}.lzo`

- Compress a file, while specifying the compression level. 0 = Worst, 9 = Best (Default level is 3):

`lzop -{{level}} {{path/to/file}}`
