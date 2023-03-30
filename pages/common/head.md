# head 
## chatgpt 
The "head" command in Linux is used to display the first few lines of a text file or output. By default, the "head" command displays the first ten lines of a file, but you can specify the number of lines to display using the "-n" option. 

The basic syntax of the "head" command is as follows:

head [OPTIONS] [FILE]

Here, "OPTIONS" are optional arguments that can be used to modify the behavior of the command, and "FILE" is the name of the file to be displayed. If no file is specified, the "head" command reads from standard input.

Some of the commonly used options for the "head" command are as follows:

- "-n": Specifies the number of lines to display. For example, "head -n 5 FILE" will display the first five lines of the file.

- "-q": Suppresses the header information that is normally displayed when more than one file is processed.

- "-v": For multiple files, displays the name of each file before the output of that file.

So, in summary, the "head" command is a useful tool for quickly viewing the beginning of a file or output, and it offers several options to customize its behavior. 

## tldr 
 
> Output the first part of files.
> More information: <https://www.gnu.org/software/coreutils/head>.

- Output the first few lines of a file:

`head -n {{count}} {{path/to/file}}`
