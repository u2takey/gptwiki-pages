# fmt 
## chatgpt 
The `fmt` command is a text formatting utility that is used to format text by breaking it into multiple lines and adding appropriate line breaks and spacing to make it more readable. Some common uses of the `fmt` command include:

1. Wrapping lines of text to a specific width:
The `fmt` command can be used to wrap long lines of text to a specific width. This can be done by specifying the maximum width using the `-w` option followed by the number of characters. For example, the command `fmt -w 80 file.txt` would wrap the text in the file.txt file to 80 characters per line.

2. Reformatting text for better readability:
The `fmt` command can also be used to reformat text for better readability. This is done by removing unnecessary line breaks and adding appropriate spacing between words and sentences. To do this, simply enter the `fmt` command followed by the name of the file containing the unformatted text. For example, the command `fmt file.txt` would reformat the contents of the file.txt file.

3. Adjusting line spacing:
The `fmt` command can also be used to adjust line spacing in a text file. This can be done by specifying the desired line spacing using the `-s` option followed by a value indicating the number of spaces to insert between lines. For example, the command `fmt -s 2 file.txt` would insert 2 spaces between each line of text in the file.txt file.

Overall, the `fmt` command is a useful utility for formatting text files in a way that makes them more readable and easier to work with. 

## tldr 
 
> Reformat a text file by joining its paragraphs and limiting the line width to given number of characters (75 by default).
> More information: <https://www.gnu.org/software/coreutils/fmt>.

- Reformat a file:

`fmt {{path/to/file}}`

- Reformat a file producing output lines of (at most) `n` characters:

`fmt -w {{n}} {{path/to/file}}`

- Reformat a file without joining lines shorter than the given width together:

`fmt -s {{path/to/file}}`

- Reformat a file with uniform spacing (1 space between words and 2 spaces between paragraphs):

`fmt -u {{path/to/file}}`
