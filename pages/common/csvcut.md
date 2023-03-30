# csvcut 
## chatgpt 
csvcut is a command line utility used to slice and filter comma-separated values (CSV) files. It is an easy-to-use tool that helps extract specific columns from a large CSV file and remove any unwanted data.

Here is an overview of some of the common commands used with csvcut:

1. -d, --delimiter: This command specifies the delimiter used in the CSV file. By default, it is a comma, but it can be a tab or a pipe character.

2. -c, --columns: This command specifies the column(s) to extract from the CSV file. Multiple columns can be specified by separating them with a comma, and ranges can be specified using a hyphen.

3. -x, --exclude: This command specifies the column(s) to exclude from the output. Similar to -c, multiple columns can be excluded by separating them with commas.

4. -f, --fields: This command works like -c and specifies the column(s) to extract, but it allows for more advanced field selection, such as regular expressions.

5. -l, --linenumbers: This command adds a line number column to the output, making it easy to track specific rows.

6. -I, --ignorecase: This command makes the filtering case-insensitive.

7. -q, --quiet: This command suppresses any warning messages and errors.

Overall, csvcut is a useful tool for managing CSV files and can make it easier to extract the specific data you need from a large dataset. 

## tldr 
 
> Filter and truncate CSV files. Like Unix's `cut` command, but for tabular data.
> Included in csvkit.
> More information: <https://csvkit.readthedocs.io/en/latest/scripts/csvcut.html>.

- Print indices and names of all columns:

`csvcut -n {{data.csv}}`

- Extract the first and third columns:

`csvcut -c {{1,3}} {{data.csv}}`

- Extract all columns **except** the fourth one:

`csvcut -C {{4}} {{data.csv}}`

- Extract the columns named "id" and "first name" (in that order):

`csvcut -c {{id,"first name"}} {{data.csv}}`
