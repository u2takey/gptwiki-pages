# q 
## chatgpt 
The command "q" by itself does not have a clear or specific meaning. It is a single letter which could potentially represent multiple commands or functions depending on the context in which it is used.

In some cases, "q" could be a shortcut for quitting a program or application. For example, in the command line interface, typing "q" can sometimes be used to exit or close out of a program or shell.

In other contexts, "q" may be used as shorthand for other commands or functions. For instance, in some programs or software, "q" could be used to denote a query or search function. In other cases, it may be used as an abbreviation for "quit", "quick", "quote", or "quiet".

Overall, the meaning of the "q" command can vary depending on the context and the specific program or application in use. Without more information or context, it is difficult to give a comprehensive description of its meaning or usage. 

## tldr 
 
> Execute SQL-like queries on .csv and .tsv files.
> More information: <https://harelba.github.io/q>.

- Query `.csv` file by specifying the delimiter as ',':

`q -d',' "SELECT * from {{path/to/file}}"`

- Query `.tsv` file:

`q -t "SELECT * from {{path/to/file}}"`

- Query file with header row:

`q -d{{delimiter}} -H "SELECT * from {{path/to/file}}"`

- Read data from `stdin`; '-' in the query represents the data from `stdin`:

`{{output}} | q "select * from -"`

- Join two files (aliased as `f1` and `f2` in the example) on column `c1`, a common column:

`q "SELECT * FROM {{path/to/file}} f1 JOIN {{path/to/other_file}} f2 ON (f1.c1 = f2.c1)"`

- Format output using an output delimiter with an output header line (note: command will output column names based on the input file header or the column aliases overridden in the query):

`q -D{{delimiter}} -O "SELECT {{column}} as {{alias}} from {{path/to/file}}"`
