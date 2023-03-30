# csv2tsv 
## chatgpt 
The `csv2tsv` command is a command-line tool that is used to convert a comma-separated values (CSV) file to a tab-separated values (TSV) file. This command is used when we need to change the delimiter in a file from a comma (,) to a tab character (\t).

Here is how to use `csv2tsv` command:

Syntax:
```
csv2tsv [options] [input file] > [output file]
```

Options:

- `-d`, `--delimiter`: Specify the delimiter to use in the input file. The default delimiter is a comma.

- `-h`, `--help`: Display the help message and exit.

- `-v`, `--version`: Display the version of the command and exit.

Input file: The name of the CSV file that needs to be converted.

Output file: The name of the TSV file that will be created after conversion.

Example:

Suppose we have a CSV file called "example.csv" with the following contents:

```
Sno,Name,Age
1,John,25
2,Emily,28
3,Leo,30
```

To convert this file to a TSV file, we use the `csv2tsv` command as follows:

```
csv2tsv example.csv > example.tsv
```

The above command reads the CSV file "example.csv", converts it to a TSV file, and writes it to the file "example.tsv".

The contents of the "example.tsv" file after conversion will be:

```
Sno     Name    Age
1       John    25
2       Emily   28
3       Leo     30
```

As you can see above, the comma delimiter in the original CSV file is replaced with a tab character in the TSV file. This makes it easier to read and work with the file data. 

## tldr 
 
> Convert CSV (comma-separated) text to TSV (tab-separated) format.
> More information: <https://github.com/eBay/tsv-utils/blob/master/README.md#csv2tsv>.

- Convert from CSV to TSV:

`csv2tsv {{path/to/input_csv1 path/to/input_csv2 ...}} > {{path/to/output_tsv}}`

- Convert field delimiter separated CSV to TSV:

`csv2tsv -c'{{field_delimiter}}' {{path/to/input_csv}}`

- Convert semicolon separated CSV to TSV:

`csv2tsv -c';' {{path/to/input_csv}}`
