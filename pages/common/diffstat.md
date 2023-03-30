# diffstat 
## chatgpt 
The `diffstat` command is a Linux tool used to generate a summary of the changes between two files or directories. It outputs a summary of the differences in a patch file format that can be read easily by humans. The summary created by `diffstat` shows the number of additions, deletions, and changes made to each file, along with the percentage of the total changes.

The syntax of the `diffstat` command is as follows:

```
$ diffstat [options] [file1] [file2]
```

Here, `file1` and `file2` are the two files or directories that need to be compared. Some of the commonly used options with `diffstat` command are:

- `-c`: Shows the context of the changes in the output.
- `-p`: Shows the patch of the changes in the output.
- `-s`: Suppresses the output for unmodified files.
- `-h`: Displays the output in a more human-readable format.

For example, to compare two files `file1.txt` and `file2.txt` and generate a summary of differences, run the following command:

```
$ diffstat file1.txt file2.txt
```

The output of this command will be a summary of the differences between the two files.

```
 file1.txt |   10 -
 file2.txt |    9 +++
 2 files changed, 9 insertions(+), 10 deletions(-)
```

This output indicates that `file1.txt` has 10 lines removed, while `file2.txt` has 9 lines added. The final line shows the overall statistics of the changes made in both files, with 9 insertions and 10 deletions in total. 

## tldr 
 
> Create a histogram from the output of the `diff` command.
> More information: <https://manned.org/diffstat>.

- Display changes in a histogram:

`diff {{file1}} {{file2}} | diffstat`

- Display inserted, deleted and modified changes as a table:

`diff {{file1}} {{file2}} | diffstat -t`
