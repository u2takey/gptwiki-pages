# xsv 
## chatgpt 
`xsv` is a command-line tool for working with CSV (Comma Separated Values) files. It supports various operations such as sorting, searching, filtering, joining, and formatting CSV files.

Here are some of the most commonly used subcommands in `xsv`:

- `cat`: Output the contents of a CSV file to the console.
- `count`: Count the number of rows in a CSV file.
- `freq`: Count the frequency of each value in a column.
- `headers`: Output the headers of a CSV file.
- `select`: Select specific columns from a CSV file.
- `sort`: Sort a CSV file by one or more columns.
- `search`: Search for a specific value or pattern in a CSV file.
- `split`: Split a single CSV file into multiple smaller files.
- `join`: Join two CSV files by matching values in a specific column.

There are many more subcommands available in `xsv`, and each one has its own set of options and flags. For detailed usage instructions, refer to the official documentation on the `xsv` website. 

## tldr 
 
> A CSV command-line toolkit written in Rust.
> More information: <https://github.com/BurntSushi/xsv>.

- Inspect the headers of a file:

`xsv headers {{path/to/file.csv}}`

- Count the number of entries:

`xsv count {{path/to/file.csv}}`

- Get an overview of the shape of entries:

`xsv stats {{path/to/file.csv}} | xsv table`

- Select a few columns:

`xsv select {{column_a,column_b}} {{path/to/file.csv}}`

- Show 10 random entries:

`xsv sample {{10}} {{path/to/file.csv}}`

- Join a column from one file to another:

`xsv join --no-case {{column_a}} {{path/to/file/a.csv}} {{column_b}} {{path/to/file/b.csv}} | xsv table`
