# truncate 
## chatgpt 
The `truncate` command is used to shorten or empty the contents of a file. It is most commonly used to clear the contents of a log file or to reduce the size of a file. The `truncate` command can be issued from a terminal or command prompt.

The basic syntax of the `truncate` command is as follows:

```
truncate [OPTION]... FILE...
```

Here, `OPTION` refers to the various command options that can be used with the `truncate` command, and `FILE` refers to the file or files that you want to truncate.

Some of the most commonly used `truncate` options are:

- `-s, --size`: Specifies the new size of the file in bytes. For example, `truncate -s 100 myfile.txt` would set the size of `myfile.txt` to 100 bytes.
- `-c, --no-create`: Prevents `truncate` from creating a new file if the specified file does not exist.
- `-o, --io-blocks`: Sets the file size in units of the I/O block size.

Note that when you truncate a file, its contents will be permanently deleted.

Examples:
- `truncate -s 0 myfile.txt` will clear the contents of `myfile.txt`.
- `truncate -s 100 myfile.txt` will reduce the size of `myfile.txt` to 100 bytes.
- `truncate -c -s 50 newfile.txt` will create a new file `newfile.txt` with a size of 50 bytes. If the file already exists, no action will be taken. 

## tldr 
 
> Shrink or extend the size of a file to the specified size.
> More information: <https://www.gnu.org/software/coreutils/truncate>.

- Set a size of 10 GB to an existing file, or create a new file with the specified size:

`truncate --size {{10G}} {{filename}}`

- Extend the file size by 50 MiB, fill with holes (which reads as zero bytes):

`truncate --size +{{50M}} {{filename}}`

- Shrink the file by 2 GiB, by removing data from the end of file:

`truncate --size -{{2G}} {{filename}}`

- Empty the file's content:

`truncate --size 0 {{filename}}`

- Empty the file's content, but do not create the file if it does not exist:

`truncate --no-create --size 0 {{filename}}`
