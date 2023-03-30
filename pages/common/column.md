# column 
## chatgpt 
The `column` command is a Unix/Linux utility that processes a file or standard input, breaks the input into columns according to specified delimiters, and displays the output in a neatly formatted table. 

Here is the syntax for using the `column` command:

```
column [options] [file]
```

The `options` allow you to specify how the columns are formatted, including the column separator, the width of each column, and the alignment of the text within each column. Some common options include:

- `-t`: Automatically determine the number of columns based on the input, instead of specifying them manually.
- `-s`: Specify the column separator (default is whitespace).
- `-c`: Specify the maximum width of each column (default is 80 characters).
- `-o`: Specify an output delimiter (default is whitespace).
- `-N`: Specify column headers.

For example, the following command will display the contents of the file `data.txt` in a table with two columns, separated by commas:

```
$ column -s , -t data.txt
```

Here, the `-s` option specifies that the columns are separated by commas, and the `-t` option tells `column` to automatically format the input into columns. 

Overall, the `column` command is a useful tool for quickly formatting and analyzing data in a clear and organized way. 

## tldr 
 
> Format standard input or a file into multiple columns.
> Columns are filled before rows; the default separator is a whitespace.
> More information: <https://manned.org/column>.

- Format the output of a command for a 30 characters wide display:

`printf "header1 header2\nbar foo\n" | column --output-width {{30}}`

- Split columns automatically and auto-align them in a tabular format:

`printf "header1 header2\nbar foo\n" | column --table`

- Specify the column delimiter character for the `--table` option (e.g. "," for CSV) (defaults to whitespace):

`printf "header1,header2\nbar,foo\n" | column --table --separator {{,}}`

- Fill rows before filling columns:

`printf "header1\nbar\nfoobar\n" | column --output-width {{30}} --fillrows`
