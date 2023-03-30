# pr 
## chatgpt 
The `pr` command is a Unix utility that is used to prepare text files for printing or viewing. It can be used to format text files in a variety of different ways and can be useful in preparing text documents for printing.

The basic syntax of the `pr` command is as follows:

```
pr [options] [file ...]
```

The options that are available for the `pr` command include:

- `-f`: This option is used to specify a filename for the output.
- `-h`: This option is used to suppress headers.
- `-l`: This option is used to specify the number of lines per page.
- `-m`: This option is used to merge files into a single output stream.
- `-n`: This option is used to number each page.
- `-o`: This option is used to specify an offset in lines from the start of the file.
- `-s`: This option is used to specify the line spacing.
- `-t`: This option is used to print a header on each page.
- `-w`: This option is used to specify the page width.

The `pr` command can be used to adjust the formatting of a text file for printing, such as changing the margins or spacing, adjusting the page size, or adding page numbers and headers. It can also be used in pipes to filter the output of other commands and prepare it for printing, such as using `ls -l | pr` to format the output of the `ls` command in a more readable way. 

## tldr 
 
> Paginate or columnate files for printing.
> More information: <https://www.gnu.org/software/coreutils/pr>.

- Print multiple files with a default header and footer:

`pr {{file1}} {{file2}} {{file3}}`

- Print with a custom centered header:

`pr -h "{{header}}" {{file1}} {{file2}} {{file3}}`

- Print with numbered lines and a custom date format:

`pr -n -D "{{format}}" {{file1}} {{file2}} {{file3}}`

- Print all files together, one in each column, without a header or footer:

`pr -m -T {{file1}} {{file2}} {{file3}}`

- Print, beginning at page 2 up to page 5, with a given page length (including header and footer):

`pr +{{2}}:{{5}} -l {{page_length}} {{file1}} {{file2}} {{file3}}`

- Print with an offset for each line and a truncating custom page width:

`pr -o {{offset}} -W {{width}} {{file1}} {{file2}} {{file3}}`
