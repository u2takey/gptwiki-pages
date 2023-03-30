# pg_dumpall 
## chatgpt 
pg_dumpall is a command-line utility program that is used for performing a database backup from a PostgreSQL server. The pg_dumpall utility dumps out all the information in all the databases in a PostgreSQL cluster, including the database globals (roles, tablespaces), and then writes the output to a file.

The basic syntax of pg_dumpall command is as follows:

```
pg_dumpall [option...] [file]
```

Here, options are used to specify various types of options for the pg_dumpall command, and file is used to specify the destination file for the backup.

Some of the most commonly used options with pg_dumpall command are:

- -U: This option specifies the PostgreSQL user name to use to connect to the server.

- -h: This option specifies the host name of the server to connect to.

- -p: This option specifies the PostgreSQL server port.

- -f: This option specifies the output file name for the backup.

- -v: This option enables verbose mode, which displays detailed output during the backup process.

For example, to perform a database backup using pg_dumpall command, you can use the following command:

```
pg_dumpall -U postgres -f backup.sql
```

This command will create a backup of all the databases in the PostgreSQL cluster, and save the output in the file named backup.sql. The -U option specifies the username to connect to the database server, which is set to "postgres" in this example.

In summary, pg_dumpall is a powerful utility program that simplifies database backup tasks in PostgreSQL. With its various options, you can customize your backup to suit your needs and protect your data from loss. 

## tldr 
 
> Extract a PostgreSQL database cluster into a script file or other archive file.
> More information: <https://www.postgresql.org/docs/current/app-pg-dumpall.html>.

- Dump all databases:

`pg_dumpall > {{path/to/file.sql}}`

- Dump all databases using a specific username:

`pg_dumpall --username={{username}} > {{path/to/file.sql}}`

- Same as above, customize host and port:

`pg_dumpall -h {{host}} -p {{port}} > {{output_file.sql}}`

- Dump all databases into a custom-format archive file with moderate compression:

`pg_dumpall -Fc > {{output_file.dump}}`

- Dump only database data into an SQL-script file:

`pg_dumpall --data-only > {{path/to/file.sql}}`

- Dump only schema (data definitions) into an SQL-script file:

`pg_dumpall -s > {{output_file.sql}}`
