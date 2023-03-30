# sqlite3 
## chatgpt 
The command "sqlite3" is used to interact with an SQLite database.

When executed in the terminal, the sqlite3 command opens the SQLite command-line shell, allowing the user to create or modify SQLite databases within the shell environment. The syntax for the SQLite command-line shell is as follows:

sqlite3 [options] [filename]

The "filename" refers to the name of the SQLite database file that you want to connect to. If the file already exists, it will be opened. If the file does not exist, it will be created.

The "options" for sqlite3 can include:

- -help: Displays a list of available options and their descriptions.
- -version: Displays the version of SQLite that is currently installed.
- -bail: Causes SQLite to exit immediately if an error occurs.
- -init filename: Specifies a filename to read initialization SQL from.
- -echo: Prints all SQL statements that are executed to the console.
- -cmd command: Executes a single SQL command in the shell.
- -csv: Enables CSV output mode for all queries.

Once you have entered the sqlite3 command with the appropriate options and filename, you will be presented with a prompt that looks like this:

sqlite>

You can then begin entering SQL commands to create, modify, or query the SQLite database. For example, you can use the following command to create a new table in the database:

CREATE TABLE mytable (id INTEGER PRIMARY KEY, name TEXT);

This command will create a new table named "mytable" with two columns: "id" (an INTEGER column) and "name" (a TEXT column). The "PRIMARY KEY" constraint on the "id" column specifies that this column will be used as the primary key for the table.

Overall, the sqlite3 command is an essential tool for working with SQLite databases from the command line. By using this command, you can quickly and easily create, modify, and query SQLite databases without requiring any additional tools or software. 

## tldr 
 
> The command-line interface to SQLite 3, which is a self-contained file-based embedded SQL engine.
> More information: <https://sqlite.org>.

- Start an interactive shell with a new database:

`sqlite3`

- Open an interactive shell against an existing database:

`sqlite3 {{path/to/database.sqlite3}}`

- Execute an SQL statement against a database and then exit:

`sqlite3 {{path/to/database.sqlite3}} '{{SELECT * FROM some_table;}}'`
