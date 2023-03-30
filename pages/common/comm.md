# comm 
## chatgpt 
The `comm` command is used in Unix/Linux operating systems to compare two sorted files line by line. It displays the lines that are common to both files, as well as the lines that are unique to each file. The `comm` command cannot compare unsorted files.

The syntax of the `comm` command is:

`comm [OPTION]... FILE1 FILE2`

Where `FILE1` and `FILE2` are the two files to compare.

Options:
- `-1`: Suppress the output of lines unique to File1.
- `-2`: Suppress the output of lines unique to File2.
- `-3`: Suppress the output of lines that are common to both files.
- `-i`: Ignore case while comparing the files.
- `-u`: Display only the unique lines from both files.
- `-z`: Use a zero byte as a line separator instead of a new line.
- `--help`: Display the command help message.

Here are some examples of using the `comm` command:

1. Compare two files and display the output in three columns: lines unique to file1, lines unique to file2, and lines in common:
```
$ comm file1.txt file2.txt
```

2. Suppress the display of lines that are common to both files:
```
$ comm -3 file1.txt file2.txt
```

3. Display only the unique lines from both files:
```
$ comm -u file1.txt file2.txt
``` 

## tldr 
 
> Select or reject lines common to two files. Both files must be sorted.
> More information: <https://www.gnu.org/software/coreutils/comm>.

- Produce three tab-separated columns: lines only in first file, lines only in second file and common lines:

`comm {{file1}} {{file2}}`

- Print only lines common to both files:

`comm -12 {{file1}} {{file2}}`

- Print only lines common to both files, reading one file from `stdin`:

`cat {{file1}} | comm -12 - {{file2}}`

- Get lines only found in first file, saving the result to a third file:

`comm -23 {{file1}} {{file2}} > {{file1_only}}`

- Print lines only found in second file, when the files aren't sorted:

`comm -13 <(sort {{file1}}) <(sort {{file2}})`
