# sdiff 
## chatgpt 
The "sdiff" command in Linux is used to show the differences between two files side by side. The command compares each line of the two files and displays the differences between them in an easy-to-read format. 

Syntax:

The basic syntax of the sdiff command is as follows:

```
sdiff [OPTIONS] file1 file2
```

Options:

The following are the options that sdiff command provides:

- -s: This option suppresses common lines between the two files.
- -w: This option sets the width of the output.
- -t: This option uses tabs to separate the output.
- -o: This option saves the output to a file instead of displaying it on the screen.

Examples:

1. Compare two files using sdiff:

```
$ sdiff file1.txt file2.txt
```

This will show the differences between file1.txt and file2.txt.

2. Compare two files and suppress common lines:

```
$ sdiff -s file1.txt file2.txt
```

This command will only display the lines that are different between file1.txt and file2.txt.

3. Compare files and save the output to a file:

```
$ sdiff -o output.txt file1.txt file2.txt
```

This command will save the output of the sdiff command to output.txt file. 

Overall, using the sdiff command can help you quickly identify and analyze differences between two files, which can be helpful in troubleshooting issues or identifying changes made between two versions of a file. 

## tldr 
 
> Compare the differences between and optionally merge 2 files.
> More information: <https://manned.org/sdiff>.

- Compare 2 files:

`sdiff {{path/to/file1}} {{path/to/file2}}`

- Compare 2 files, ignoring all tabs and whitespace:

`sdiff -W {{path/to/file1}} {{path/to/file2}}`

- Compare 2 files, ignoring whitespace at the end of lines:

`sdiff -Z {{path/to/file1}} {{path/to/file2}}`

- Compare 2 files in a case-insensitive manner:

`sdiff -i {{path/to/file1}} {{path/to/file2}}`

- Compare and then merge, writing the output to a new file:

`sdiff -o {{path/to/merged_file}} {{path/to/file1}} {{path/to/file2}}`
