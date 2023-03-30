# csvtool 
## chatgpt 
`csvtool` is a command-line tool that is used to manipulate and analyze CSV (Comma-Separated Values) files. It is a versatile tool that can perform a wide range of operations on CSV files, such as sorting, filtering, joining, splitting, and converting formats.

The csvtool command is run from the command-line interface (CLI) of the operating system by specifying the desired operation and the file to be processed. The syntax of the command varies depending on the operation being performed, but typically it follows this format:

$ csvtool [operation] [options] [input_file] [output_file]

Here are some examples of the csvtool command syntax with different operations:

1. Sorting: sorts a CSV file based on one or more columns.

$ csvtool sort [options] [input_file] [output_file]

Options:

-c, --columns: specifies the columns to sort by.

-r, --reverse: sorts in reverse order.

-u, --unique: removes duplicate rows.

2. Filtering: extracts rows from a CSV file that match a specified condition.

$ csvtool filter [options] [input_file] [output_file]

Options:

-c, --column: specifies the column to filter by.

-r, --regexp: specifies the regular expression to match.

-i, --invert: selects rows that do not match the condition.

3. Joining: merges two or more CSV files based on a common column.

$ csvtool join [options] [input_file1] [input_file2] [...] [output_file]

Options:

-c, --common: specifies the common column(s) to join on.

-l, --left: includes all rows from the first file.

-r, --right: includes all rows from the second file.

-i, --inner: includes only rows that match in both files.

-cf, --common-format: specifies the format of the common column(s).

4. Splitting: breaks a CSV file into smaller files based on a specified column.

$ csvtool split [options] [input_file] [output_directory]

Options:

-c, --column: specifies the column to split by.

-n, --name-template: specifies the name template for the output files.

-f, --format: specifies the format for the output files.

5. Converting: convert a CSV file to another format, such as TSV, HTML, or JSON.

$ csvtool format [options] [input_file] [output_file]

Options:

-d, --delimiter: specifies the delimiter character for the output file.

-q, --quote: specifies the quote character for the output file.

-t, --type: specifies the output file type (TSV, HTML, JSON, etc.).

These are just a few examples of the many operations that can be performed with the `csvtool` command. By using the different options and combining them with pipe commands, users can create complex data processing workflows that manipulate and analyze large CSV files efficiently. 

## tldr 
 
> Utility to filter and extract data from CSV formatted sources.
> More information: <https://github.com/maroofi/csvtool>.

- Extract the second column from a CSV file:

`csvtool --column {{2}} {{path/to/file.csv}}`

- Extract the second and fourth columns from a CSV file:

`csvtool --column {{2,4}} {{path/to/file.csv}}`

- Extract lines from a CSV file where the second column exactly matches 'Foo':

`csvtool --column {{2}} --search '{{^Foo$}}' {{path/to/file.csv}}`

- Extract lines from a CSV file where the second column starts with 'Bar':

`csvtool --column {{2}} --search '{{^Bar}}' {{path/to/file.csv}}`

- Find lines in a CSV file where the second column ends with 'Baz' and then extract the third and sixth columns:

`csvtool --column {{2}} --search '{{Baz$}}' {{path/to/file.csv}} | csvtool --no-header --column {{3,6}}`
