# csvkit 
## chatgpt 
CSVkit is an open-source command-line tool that provides a suite of utilities for working with CSV files. It can be used to perform many common data manipulation tasks, such as filtering and transforming data, joining multiple CSV files, and exporting data to various file formats.

To use CSVkit, you need to have Python installed on your system. Once installed, you can install CSVkit using the following command:

```
pip install csvkit
```

After installation, you can use various commands provided by CSVkit in the terminal. Here are some common commands:

1. **csvcut:** This command can be used to extract columns from a CSV file. The syntax is:

```
csvcut -c column1,column2 input.csv > output.csv
```

2. **csvgrep:** This command can be used to filter rows from a CSV file that match a given pattern. The syntax is:

```
csvgrep -c column -m pattern input.csv > output.csv
```

3. **csvjoin:** This command can be used to join two CSV files based on a common column. The syntax is:

```
csvjoin --left -c column input1.csv input2.csv > output.csv
```

4. **csvstack:** This command can be used to stack multiple CSV files on top of each other. The syntax is:

```
csvstack input1.csv input2.csv > output.csv
```

5. **csvformat:** This command can be used to convert a CSV file to a different format, such as JSON or SQL. The syntax is:

```
csvformat -j input.csv > output.json
```

Overall, CSVkit provides a powerful set of tools for working with CSV files, which can make data manipulation and analysis easier and more efficient. 

## tldr 
 
> Manipulation toolkit for CSV files.
> See the individual commands: `csvclean`, `csvcut`, `csvformat`, `csvgrep`, `csvlook`, `csvpy`, `csvsort`, `csvstat`.
> More information: <https://csvkit.readthedocs.io/en/0.9.1/cli.html>.

- Run a command on a CSV file with a custom delimiter:

`{{cmd}} -d {{delimiter}} {{filename.csv}}`

- Run a command on a CSV file with a tab as a delimiter (overrides -d):

`{{cmd}} -t {{filename.csv}}`

- Run a command on a CSV file with a custom quote character:

`{{cmd}} -q {{quote_char}} {{filename.csv}}`

- Run a command on a CSV file with no header row:

`{{cmd}} -H {{filename.csv}}`
