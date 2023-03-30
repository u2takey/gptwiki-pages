# cat 
## chatgpt 
The "cat" command in Linux is short for "concatenate", which means to join two or more strings of text together into a single file. In its most basic form, the "cat" command is used to display the contents of a text file in the terminal window.

Syntax: cat [options] [file(s)]

The "options" are additional instructions that tell the command what to do, and could include flags to add line numbering, show non-printing characters, or display the contents in reverse order. 

If you run the "cat" command without any options, it will simply output the contents of the specified file(s) to the terminal. 

Examples:

1. Display the contents of a file on the terminal: cat filename.txt

2. Combine two files and display the contents: cat file1.txt file2.txt

3. Add line numbers to the output: cat -n filename.txt

4. Display non-printing characters: cat -v filename.txt 

5. Display the contents of a file in reverse order: cat filename.txt | rev 

Overall, the cat command is a versatile tool that can be used for a wide variety of tasks, such as displaying text files, reading input from the standard input stream, or concatenating multiple files into a single file. 

## tldr 
 
> Print and concatenate files.
> More information: <https://www.gnu.org/software/coreutils/cat>.

- Print the contents of a file to the standard output:

`cat {{path/to/file}}`

- Concatenate several files into an output file:

`cat {{path/to/file1 path/to/file2 ...}} > {{path/to/output_file}}`

- Append several files to an output file:

`cat {{path/to/file1 path/to/file2 ...}} >> {{path/to/output_file}}`

- Copy the contents of a file into an output file without buffering:

`cat -u {{/dev/tty12}} > {{/dev/tty13}}`

- Write `stdin` to a file:

`cat - > {{path/to/file}}`
