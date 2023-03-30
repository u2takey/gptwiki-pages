# split 
## chatgpt 
The `split` command is a Unix/Linux command that is used to split a file into smaller pieces or chunks.

Syntax:

`split [options] filename`

Here, `filename` is the name of the file to be split into smaller pieces.

Options:

- `-b`: This option is used to specify the size of each chunk in bytes. The default size is 1,048,576 bytes (1 MB).
For example: `split -b 1024 file.txt` will split the file "file.txt" into chunks of 1 KB each.

- `-l`: This option is used to specify the number of lines in each chunk. For example, `split -l 100 file.txt` will split the file "file.txt" into chunks of 100 lines each.

- `-d`: This option is used to add numerical suffixes to the output files instead of alphabetic suffixes. For example, `split -d file.txt` will generate files with names like file.txt00, file.txt01, file.txt02, etc.

- `-a`: This option is used to specify the length of the numerical suffixes. For example, `split -a 3 file.txt` will generate files with names like file.txt000, file.txt001, file.txt002, etc.

- `-p`: This option is used to split the file at specified regular expressions. For example, `split -p 'regex' file.txt` will split the file "file.txt" at every occurrence of 'regex'.

- `--verbose`: This option is used to display the progress of the split operation.

Once the split command is executed, it will create multiple files with the same name as the original file, but with a unique suffix. These files contain the smaller chunks of the original file. 

## tldr 
 
> Split a file into pieces.
> More information: <https://www.gnu.org/software/coreutils/split>.

- Split a file, each split having 10 lines (except the last split):

`split -l {{10}} {{path/to/file}}`

- Split a file into 5 files. File is split such that each split has same size (except the last split):

`split -n {{5}} {{path/to/file}}`

- Split a file with 512 bytes in each split (except the last split; use 512k for kilobytes and 512m for megabytes):

`split -b {{512}} {{path/to/file}}`

- Split a file with at most 512 bytes in each split without breaking lines:

`split -C {{512}} {{path/to/file}}`
