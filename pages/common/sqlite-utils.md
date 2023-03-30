# sqlite-utils 
## chatgpt 
`sqlite-utils` is a command-line utility for working with SQLite databases. It is a Python package that provides a set of command-line tools for creating, updating, querying and manipulating SQLite databases.

Here are some of the most common commands provided by `sqlite-utils`:

- `sqlite-utils create <database_file>` - creates a new SQLite database file
- `sqlite-utils insert <database_file> <table_name> <data.json>` - inserts data from a JSON file into a new or existing table
- `sqlite-utils query <database_file> "SELECT * FROM <table_name>"` - runs a SQL query against the database and prints the result to the console
- `sqlite-utils serve <database_file> -p 8080` - starts a web server that provides a REST API for querying the database
- `sqlite-utils view <database_file> <table_name>` - displays a table of data from the database in the terminal

`sqlite-utils` is a versatile tool that can be used for a range of tasks, from simple data queries to building web applications that interact with an SQLite database. Its user-friendly command-line interface makes it easy to get started with SQLite and begin working with data. 

## tldr 
 
> Command-line tool used to manipulate SQLite databases in a number of different ways.
> More information: <https://sqlite-utils.datasette.io/en/stable/cli.html>.

- Create a database:

`sqlite-utils create-database {{path/to/database.db}}`

- Create a table:

`sqlite-utils create-table {{path/to/database.db}} {{table_name}} {{id integer name text height float photo blob --pk id}}`

- List tables:

`sqlite-utils tables {{path/to/database.db}}`

- Upsert a record:

`{{echo '[ {"id": 1, "name": "Linus Torvalds"}, {"id": 2, "name": "Steve Wozniak"}, {"id": 3, "name": "Tony Hoare"} ]'}} | sqlite-utils upsert {{path/to/database.db}} {{table_name}} - {{--pk id}}`

- Select records:

`sqlite-utils rows {{path/to/database.db}} {{table_name}}`

- Delete a record:

`sqlite-utils query {{path/to/database.db}} "{{delete from table_name where name = 'Tony Hoare'}}"`

- Drop a table:

`sqlite-utils drop-table {{path/to/database.db}} {{table_name}}`

- Show help information:

`sqlite-utils -h`
