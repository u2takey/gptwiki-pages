# cmp 
## chatgpt 
The "cmp" command is a utility command available in Unix and Linux operating systems that are used for comparing two files byte by byte. 

The general syntax of the command is:

cmp [option] file1 file2

Where "file1" and "file2" are the two files to be compared. 

Some of the most commonly used options with the cmp command are:

- -s: This option makes the command silent and only reports if the files are different, without displaying any output.
- -l: This option shows the byte number and the differing byte value of the files.
- -i n: This option compares the files from byte "n" onwards instead of from the beginning of the files.
- -n bytes: This option limits the comparison to the first "n" bytes of the files.

When executing the cmp command, it compares two files byte-by-byte and displays the first byte in which the two files differ. If the files are identical, no output is displayed. The cmp command is useful when one needs to verify the consistency of a file after it has been transferred over a network or between storage devices. 

## tldr 
 
> Compare two files byte by byte.
> More information: <https://www.gnu.org/software/diffutils/manual/html_node/Invoking-cmp.html>.

- Output char and line number of the first difference between two files:

`cmp {{path/to/file1}} {{path/to/file2}}`

- Output info of the first difference: char, line number, bytes, and values:

`cmp --print-bytes {{path/to/file1}} {{path/to/file2}}`

- Output the byte numbers and values of every difference:

`cmp --verbose {{path/to/file1}} {{path/to/file2}}`

- Compare files but output nothing, yield only the exit status:

`cmp --quiet {{path/to/file1}} {{path/to/file2}}`
