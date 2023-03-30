# brotli 
## chatgpt 
Brotli is a command that is used to compress and decompress data using the Brotli compression algorithm. The Brotli algorithm was developed by Google and is designed to provide faster and more efficient compression than other algorithms, such as Gzip or Deflate.

The brotli command can be used in a variety of ways. Here are a few examples:

To compress a file:

```
brotli file.txt
```

This will compress the file.txt file using Brotli and create a new file called file.txt.br in the same directory.

To decompress a file:

```
brotli -d file.txt.br
```

This will decompress the file.txt.br file and create a new file called file.txt in the same directory.

To compress multiple files:

```
brotli file1.txt file2.txt file3.txt
```

This will compress all three files using Brotli and create new files with the .br extension in the same directory.

To compress a directory:

```
brotli -r myfolder/
```

This will compress all files in the myfolder directory and create new compressed files with the .br extension in the same directory.

Overall, the brotli command is a useful tool for compressing and decompressing files and directories using the efficient Brotli compression algorithm. 

## tldr 
 
> Compress/uncompress files with Brotli compression.
> More information: <https://github.com/google/brotli>.

- Compress a file, creating a compressed version next to the file:

`brotli {{file.ext}}`

- Decompress a file, creating an uncompressed version next to the file:

`brotli -d {{file.ext}}.br`

- Compress a file specifying the output filename:

`brotli {{file.ext}} -o {{compressed_file.ext.br}}`

- Decompress a Brotli file specifying the output filename:

`brotli -d {{compressed_file.ext.br}} -o {{file.ext}}`

- Specify the compression level. 1=Fastest (Worst), 11=Slowest (Best):

`brotli -q {{11}} {{file.ext}} -o {{compressed_file.ext.br}}`
