# psql 
## chatgpt 
psql is a command-line interface (CLI) application for interacting with PostgresSQL databases. When you run the psql command in the terminal, it establishes a connection to a PostgreSQL server, and opens a psql prompt for you to issue commands to the server. 

Here are some common options and arguments you can pass to the psql command:

- -U, --username: Specifies the username to connect as.
- -d, --dbname: Specifies the name of the database to connect to.
- -h, --host: Specifies the host name or IP address of the server.
- -p, --port: Specifies the port number of the server.
- -c, --command: Specifies a single command to run instead of opening a prompt.
- -f, --file: Specifies a file of SQL commands to execute.

When you run the psql command without any options, it tries to connect to a PostgreSQL server running on the same machine, using your current username and the default database name (which is usually your username). It opens a psql prompt where you can type SQL commands and press Enter to execute them. 

Here are some common psql commands you can use at the prompt:

- \l: Lists all available databases.
- \c dbname: Connects to a different database.
- \q: Quits psql and closes the connection.
- \i filename: Executes the SQL commands in a file.
- \d table_name: Describes the structure of a table.
- \dt: Lists all tables in the current database.

Overall, the psql command is a powerful tool for working with PostgreSQL databases, allowing you to create and manipulate tables, queries data, and manage users and permissions. 

## tldr 
 
> PostgreSQL command-line client.
> More information: <https://www.postgresql.org/docs/current/app-psql.html>.

- Connect to the database. By default, it connects to the local socket using port 5432 with the currently logged in user:

`psql {{database}}`

- Connect to the database on given server host running on given port with given username, without a password prompt:

`psql -h {{host}} -p {{port}} -U {{username}} {{database}}`

- Connect to the database; user will be prompted for password:

`psql -h {{host}} -p {{port}} -U {{username}} -W {{database}}`

- Execute a single SQL query or PostgreSQL command on the given database (useful in shell scripts):

`psql -c '{{query}}' {{database}}`

- Execute commands from a file on the given database:

`psql {{database}} -f {{file.sql}}`
