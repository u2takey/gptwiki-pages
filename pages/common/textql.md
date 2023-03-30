# textql 
## chatgpt 
Textql is a command-line tool used to execute SQL queries on structured text files. It allows users to manipulate and query CSV and TSV files using SQL commands. Here's a detailed explanation of its usage:

1. Installation: First, the command needs to be installed. Textql can be installed via the command-line interface using pip. Simply run "pip install textql" and it will install the textql package.

2. Running a query: Once installed, you can start using the textql command. To run a query, navigate to the directory where the text/csv file is located, then run "textql -header -sql 'SELECT * FROM FILENAME.csv'" to select everything from the csv file.

3. File types: The textql command supports several file types, including CSV, TSV, and fixed-width text files. You can specify the file type by using the --delimiter option followed by the delimiter character. For example, if the file is a tab-separated file, you can use "textql -header -delimiter '\t' -sql 'SELECT * FROM FILENAME.tsv'" to query the tsv file.

4. Commands: The textql command supports basic SQL commands such as select, where, group by, order by, and join. You can use these commands to manipulate and query data from the specified file.

5. Output: The output of the query is displayed in the console, but you can also specify an output file by using the -output option followed by the output file name. For example, "textql -header -sql 'SELECT * FROM FILENAME.csv' -output output.csv" will create a new csv file with the output of the query.

Overall, textql is a powerful and easy-to-use tool for querying and manipulating structured text files using SQL commands. 

## tldr 
 
> Execute SQL against structured text like csv or tsv files.
> More information: <https://github.com/dinedal/textql>.

- Print the lines in the specified `.csv` file that match a SQL query to `stdout`:

`textql -sql "{{SELECT * FROM filename}}" {{path/to/filename.csv}}`

- Query `.tsv` file:

`textql -dlm=tab -sql "{{SELECT * FROM filename}}" {{path/to/filename.tsv}}`

- Query file with header row:

`textql -dlm={{delimiter}} -header -sql "{{SELECT * FROM filename}}" {{path/to/filename.csv}}`

- Read data from `stdin`:

`cat {{path/to/file}} | textql -sql "{{SELECT * FROM stdin}}"`

- Join two files on a specified common column:

`textql -header -sql "SELECT * FROM {{file1}} JOIN {{file2}} ON {{file1}}.{{c1}} = {{file2}}.{{c1}} LIMIT {{10}}" -output-header {{path/to/file1.csv}} {{path/to/file2.csv}}`

- Format output using an output delimiter with an output header line:

`textql -output-dlm={{delimiter}} -output-header -sql "SELECT {{column}} AS {{alias}} FROM {{filename}}" {{path/to/filename.csv}}`
