# pg_isready 
## chatgpt 
`pg_isready` is a command-line utility used to check the status of a PostgreSQL server. The utility sends a connection request to the specified PostgreSQL server and waits for a response. If the server responds with a valid response, the utility reports that the server is up and running. Otherwise, it reports that the server is not ready.

The command can be used with various options to specify the server hostname, port, and database name. Here are some examples of the command and its options:

- `pg_isready` - checks the default PostgreSQL server on the local machine using default options.

- `pg_isready -h myserver -p 5432 -d mydb` - checks the PostgreSQL server with hostname "myserver", port number "5432", and database name "mydb".

The output of the command includes the server status, as well as information about the server version, hostname, port, and database name. The output format can be customized using options such as "--quiet" or "--timeout".

In general, `pg_isready` is a useful utility for monitoring PostgreSQL server availability and readiness. It can be used in scripts to automate server monitoring or to diagnose connection problems. 

## tldr 
 
> Check the connection status of a PostgreSQL server.
> More information: <https://www.postgresql.org/docs/current/app-pg-isready.html>.

- Check connection:

`pg_isready`

- Check connection with a specific hostname and port:

`pg_isready --host={{hostname}} --port={{port}}`

- Check connection displaying a message only when the connection fails:

`pg_isready --quiet`
