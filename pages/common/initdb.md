# initdb 
## chatgpt 
The "initdb" command is a utility program used to create a new PostgreSQL database cluster. It initializes a new PostgreSQL database instance with a set of default settings and creates the necessary directories and files for the database cluster.

More specifically, the "initdb" command performs the following tasks:

1. Creates a new PostgreSQL database cluster directory in the specified path.
2. Initializes the necessary files required to run a PostgreSQL database cluster, such as the pg_hba.conf (configuration file for host-based authentication) and postgresql.conf (configuration file for the PostgreSQL server).
3. Creates the initial system tables required for the database cluster to function properly.
4. Sets up the default database encoding, collation, and character classification settings.

To use the "initdb" command, you must have administrator privileges on the server. The basic syntax of the command is as follows:

```
initdb [option ...] [directory]
```

Here, the "options" parameter can be used to specify additional settings, such as the default encoding, locale, and data directory. The "directory" parameter specifies the path where the new database cluster will be created.

Overall, the "initdb" command is an essential utility for starting a fresh PostgreSQL database cluster from scratch. 

## tldr 
 
> Create a PostgreSQL database on disk.
> More information: <https://www.postgresql.org/docs/9.5/app-initdb.html>.

- Create a database at `/usr/local/var/postgres`:

`initdb -D /usr/local/var/postgres`
