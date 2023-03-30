# diff 
## chatgpt 
The command "diff" is a built-in command in Unix and Unix-like operating systems that is used to compare the contents of two files and identify the differences between them. The name "diff" is short for "difference".

Syntax: diff [option] file1 file2

Option: diff command offers a number of options, that modify the way in which it compares two files. 

Some of the commonly used options:

-c: This option tells diff to produce a context diff, which shows several lines of the files surrounding the lines that differ.

-u: This option tells diff to produce a unified diff, which presents the differences in a more compact and easily readable format.

-i: ignore case differences in the files being compared.

-b: ignore white spaces and blank lines while comparing the files.

-q: Output only whether files differ.

Output: The output of the diff command displays a list of the differences between the two files, with each difference indicated by a set of codes.

Examples:

1. To compare two files file1.txt and file2.txt and output the differences to the terminal:

   diff file1.txt file2.txt

2. To compare two files file1.txt and file2.txt and output only whether the files differ or not:

   diff -q file1.txt file2.txt

3. To ignore the case differences between files file1.txt and file2.txt:

   diff -i file1.txt file2.txt

4. To ignore blank lines and white spaces in files file1.txt and file2.txt:

   diff -b file1.txt file2.txt

Note: The diff command is commonly used in software development to compare different versions of source code, as well as for finding differences between configuration files and text documents. 

## tldr 
 
> Compare files and directories.
> More information: <https://man7.org/linux/man-pages/man1/diff.1.html>.

- Compare files (lists changes to turn `old_file` into `new_file`):

`diff {{old_file}} {{new_file}}`

- Compare files, ignoring white spaces:

`diff --ignore-all-space {{old_file}} {{new_file}}`

- Compare files, showing the differences side by side:

`diff --side-by-side {{old_file}} {{new_file}}`

- Compare files, showing the differences in unified format (as used by `git diff`):

`diff --unified {{old_file}} {{new_file}}`

- Compare directories recursively (shows names for differing files/directories as well as changes made to files):

`diff --recursive {{old_directory}} {{new_directory}}`

- Compare directories, only showing the names of files that differ:

`diff --recursive --brief {{old_directory}} {{new_directory}}`

- Create a patch file for Git from the differences of two text files, treating nonexistent files as empty:

`diff --text --unified --new-file {{old_file}} {{new_file}} > {{diff.patch}}`
