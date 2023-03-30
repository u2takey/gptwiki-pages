# cut 
## chatgpt 
The "cut" command is a Linux/Unix command that is used to extract specific sections (columns) of text from a file or a stream. It cuts out a designated part of each line of a file or standard input, and then displays the result on the standard output.

The syntax of the cut command is as follows:

cut [OPTIONS] [FILE]

Here, options represent the different ways in which the command can be customized to suit different requirements.

Some of the commonly used options of the cut command are:

- -c: This option is used to select specific characters from each line of a file or input stream. For example, "cut -c 1-3" would select the first three characters of each line.
- -f: This option is used to select specific fields from each line of a file or input stream. The fields are separated by a delimiter, which can be defined using the -d option. For example, "cut -d',' -f 1,3" would select the first and third fields of each line, assuming that the fields are separated by commas.
- -d: This option is used to specify a custom delimiter for use with the -f option. For example, "cut -d':' -f 1" would select the first field of each line, assuming that the fields are separated by colons.

Some other options of the cut command include the ability to suppress lines that do not contain the specified delimiter, and the ability to output only the specified sections of each line, without any additional formatting.

Overall, the cut command is a powerful tool that is widely used in Linux/Unix environments for extracting specific pieces of information from text files and streams. 

## tldr 
 
> Cut out fields from `stdin` or files.
> More information: <https://www.gnu.org/software/coreutils/cut>.

- Print a specific character/field range of each line:

`{{command}} | cut --{{characters|fields}}={{1|1,10|1-10|1-|-10}}`

- Print a range of each line with a specific delimiter:

`{{command}} | cut --delimiter="{{,}}" --{{fields}}={{1}}`

- Print a range of each line of the specific file:

`cut --{{characters}}={{1}} {{path/to/file}}`
