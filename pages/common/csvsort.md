# csvsort 
## chatgpt 
csvsort is a command-line tool used to sort a CSV (Comma Separated Value) file based on one or more columns. When executed, the command reads the CSV file and sorts the rows based on the specified columns. Here is a detailed explanation of the various options and arguments that can be used with the csvsort command:

Syntax: csvsort [OPTIONS] [FILE]

Options:

- -c, --column=FIELDNAMES: This option specifies the name of the column(s) based on which sorting needs to be done. Multiple columns can be specified by separating them with a comma.

- -n, --numeric: This option is used when sorting is to be done based on numeric values instead of string values.

- -r, --reverse: This option sorts the file in reverse order (Descending order).

- -h, --no-header-row: This option is used when the CSV file does not contain a header row.

- -o, --output=FILE: This option is used to specify the output file. If not specified, the output is printed to the console.

- -q, --quote: This option is used to specify the quote character used in the CSV file.

- --skip-lines=NUM: This option is used to skip the specified number of lines at the beginning of the CSV file.

Arguments:

- FILE: This is the name of the CSV file that needs to be sorted.

Example usage:

$ csvsort -c Name,Age data.csv

This command sorts the data.csv file based on the Name column first, and then the Age column. The output is printed to the console.

$ csvsort -c Name -r -o sorted.csv data.csv

This command sorts the data.csv file based on the Name column in reverse order, and outputs the sorted data to a file named sorted.csv. 

## tldr 
 
> Sorts CSV files.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvsort.html>.

- Sort a CSV file by column 9:

`csvsort -c {{9}} {{data.csv}}`

- Sort a CSV file by the "name" column in descending order:

`csvsort -r -c {{name}} {{data.csv}}`

- Sort a CSV file by column 2, then by column 4:

`csvsort -c {{2,4}} {{data.csv}}`

- Sort a CSV file without inferring data types:

`csvsort --no-inference -c {{columns}} {{data.csv}}`
