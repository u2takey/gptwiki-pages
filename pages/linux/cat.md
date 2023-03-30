# cat 
## chatgpt 
The "cat" command is a command-line utility in Linux and Unix-based operating systems that is short for "concatenate". The primary use of the cat command is to display the contents of one or more files on the command line. It can also be used to create, modify, or combine files. 

Here are some common uses of the cat command: 

1. Displaying the contents of a file: To display the contents of a file on the command line, simply type "cat" followed by the file name. For example: 

    cat myfile.txt

This will display the contents of the file "myfile.txt" on the command line. 

2. Combining two or more files: You can use the cat command to combine two or more files into a single file. For example: 

    cat file1.txt file2.txt > combinedfile.txt 

This will combine the contents of "file1.txt" and "file2.txt" into a single file called "combinedfile.txt" using the output redirection operator (>). 

3. Appending to a file: You can also use the cat command to append the contents of one file to another file. For example: 

    cat file1.txt >> file2.txt 

This will append the contents of "file1.txt" to the end of "file2.txt" using the output redirection operator (>>). 

There are many other uses for the cat command, and it has many options and variations. For more detailed information, you can check out the manual page for cat by typing "man cat" on the command line. 

## tldr 
 
> Print and concatenate files.
> More information: <https://www.gnu.org/software/coreutils/cat>.

- Print the contents of a file to the standard output:

`cat {{path/to/file}}`

- Concatenate several files into an output file:

`cat {{path/to/file1 path/to/file2 ...}} > {{path/to/output_file}}`

- Append several files to an output file:

`cat {{path/to/file1 path/to/file2 ...}} >> {{path/to/output_file}}`

- Copy the contents of a file into an output file in [u]nbuffered mode:

`cat -u {{/dev/tty12}} > {{/dev/tty13}}`

- Write `stdin` to a file:

`cat - > {{path/to/file}}`

- [n]umber all output lines:

`cat -n {{path/to/file}}`

- Display non-printable and whitespace characters (with `M-` prefix if non-ASCII):

`cat -v -t -e {{path/to/file}}`
