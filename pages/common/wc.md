# wc 
## chatgpt 
The "wc" (word count) command is a command-line utility in Unix and Linux systems that is used to display the number of lines, words, and characters in a file. The basic syntax of the "wc" command is:

wc [options] [file(s)]

Here, "options" are the additional parameters that can be used to modify the output of the command, and "file(s)" is the name(s) of the file(s) for which the word count is to be displayed.

By default, the "wc" command displays the number of lines, words, and characters in a file. For example:

$ wc myfile.txt

This will display output in the following form:

  10  50 300 myfile.txt

Here, the first column represents the number of lines in the file, the second column represents the number of words, and the third column represents the number of characters.

The "wc" command supports several options that can be used to modify its behavior. Some common options are:

-c: Displays the number of bytes in a file.
-l: Displays the number of lines in a file.
-m: Displays the number of characters in a file.
-w: Displays the number of words in a file.

For example, if you want to display only the number of lines in a file, you can use the following command:

$ wc -l myfile.txt

This will display output in the following form:

  10 myfile.txt

In this case, the second column represents the number of lines in the file.

Overall, the "wc" command is a useful tool for quickly analyzing the content of text files from the command line. 

## tldr 
 
> Count lines, words, and bytes.
> More information: <https://www.gnu.org/software/coreutils/wc>.

- Count all lines in a file:

`wc --lines {{path/to/file}}`

- Count all words in a file:

`wc --words {{path/to/file}}`

- Count all bytes in a file:

`wc --bytes {{path/to/file}}`

- Count all characters in a file (taking multi-byte characters into account):

`wc --chars {{path/to/file}}`

- Count all lines, words and bytes from `stdin`:

`{{find .}} | wc`

- Count the length of the longest line in number of characters:

`wc --max-line-length {{path/to/file}}`
