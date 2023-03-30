# join 
## chatgpt 
The "join" command is used to combine the contents of two separate files by matching a specific field or column. The files must be sorted in a specific order for the join function to work correctly.

The basic syntax of the "join" command is:

join [options] file1 file2

Some of the common options used with the command are:

- -1, -2: specifies the field number for file1 and file2 to be used for the join operation.
- -t: specifies the delimiter used to separate fields in both files.
- -a: specifies whether to include all lines from file1, file2, or both in the output.
- -o: specifies the format of the output when joining two files.
- -v: specifies whether to print only unmatched lines.

For example, to join two files named "file1.txt" and "file2.txt" using the second field as the matching key, the command would be:

join -1 2 -2 2 file1.txt file2.txt

This command will join the two files on the second field and produce a combined output based on the matching keys. If any matching keys are not found, those lines will not be included in the output. Additionally, the options can be used to include all lines from either file or only unmatched lines as needed. 

## tldr 
 
> Join lines of two sorted files on a common field.
> More information: <https://www.gnu.org/software/coreutils/join>.

- Join two files on the first (default) field:

`join {{file1}} {{file2}}`

- Join two files using a comma (instead of a space) as the field separator:

`join -t {{','}} {{file1}} {{file2}}`

- Join field3 of file1 with field1 of file2:

`join -1 {{3}} -2 {{1}} {{file1}} {{file2}}`

- Produce a line for each unpairable line for file1:

`join -a {{1}} {{file1}} {{file2}}`

- Join a file from `stdin`:

`cat {{path/to/file1}} | join - {{path/to/file2}}`
