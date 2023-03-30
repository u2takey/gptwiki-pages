# zcmp 
## chatgpt 
The zcmp command is a Linux command used to compare two compressed files. It is similar to the cmp command but specifically designed to work with compressed files.

The syntax of the command is as follows:

zcmp [options] file1 file2

Options:
* -c: display the first line where the files differ
* -i: ignore case when comparing the files
* -l: display the byte number and value of each differing byte
* -s: suppress error messages

The zcmp command can compare various compressed file types like .gz, .bz2, .xz, .z and .Z. When comparing two compressed files, zcmp first decompresses them and then compares the contents. The decompression is done automatically by the command.

If the contents of the two files are identical, the command will output nothing and the exit status will be 0. If the two files differ, the first differing byte offset and its value are displayed by default, but this behavior can be modified by the options.

In summary, zcmp is a useful command for comparing compressed files and quickly identifying differences between them. 

## tldr 
 
> Compare compressed files.
> More information: <https://manned.org/zcmp>.

- Invoke `cmp` on two files compressed via `gzip`:

`zcmp {{path/to/file1.gz}} {{path/to/file2.gz}}`

- Compare a file to its gzipped version (assuming `.gz` exists already):

`zcmp {{path/to/file}}`
