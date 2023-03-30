# mac2unix 
## chatgpt 
The command 'mac2unix' is used to convert text files that are formatted in Macintosh line endings to Unix line endings.

Macintosh line endings refer to the way text files are formatted on Macintosh computers. In these files, each line of text is separated by a single carriage return (CR) character (ASCII code 13).

Unix line endings, on the other hand, refer to the way text files are formatted on Unix and Linux systems. In Unix files, each line of text is separated by a single line feed (LF) character (ASCII code 10).

When a text file with Macintosh line endings is opened in a Unix-based editor, the editor may not recognize the Macintosh line endings and display the entire file as a single, long line. The 'mac2unix' command is used to convert the carriage return (CR) character to a line feed (LF) character to ensure the file is properly formatted for Unix-based editors.

The command can be run in the Terminal or command prompt by providing the file name as an argument to the command. For example:

$ mac2unix file.txt

This command will convert the file 'file.txt' from Macintosh line endings to Unix line endings. 

## tldr 
 
> Change macOS-style line endings to Unix-style.
> Replaces CR with LF.
> More information: <https://waterlan.home.xs4all.nl/dos2unix.html>.

- Change the line endings of a file:

`mac2unix {{filename}}`

- Create a copy with Unix-style line endings:

`mac2unix -n {{filename}} {{new_filename}}`
