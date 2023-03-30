# pg_dump 
## chatgpt 
pg_dump is a command-line utility in PostgreSQL that enables you to export a database or specific database objects to a file. The command is used to create a database backup that can be used to restore the database in case of data loss or corruption.

Here is the syntax of the pg_dump command:

```pg_dump [dbname]```

* `dbname` is the name of the database to be dumped. If this is not specified, it will default to the current user's database.

pg_dump command can be used with various options to specify what to export and how to export it. Here are a few common options:

1. `-f`: It allows you to save the dump output in a file. For example, `-f backup.sql` will save the output in the file named "backup.sql".

2. `-t`: It allows you to specify the table or tables to be exported. For example, `-t table1` will export only the "table1" table.

3. `-Fc`: It refers to the custom format which is compressed by default and is recommended for larger databases.

4. `-Z`: It specifies the level of compression that needs to be applied to the custom format dumps. For example, `-Z 9` specifies the highest level of compression.

5. `-U`: It specifies the username of the database owner or superuser to connect to the database.

6. `-p`: It specifies the port number on which the database is listening.

By default, pg_dump exports only the database objects, but not the data. To include data, you can use the `-a` option. If you want to dump the schema only and exclude data, you can use the -s option.

In summary, pg_dump is a powerful command-line utility in PostgreSQL that enables users to create database backups and export specific database objects using various options. It is a useful tool to safeguard your data and ensure that it can be recovered if data loss or corruption occurs. 

## tldr 
 
> Extract a PostgreSQL database into a script file or other archive file.
> More information: <https://www.postgresql.org/docs/current/app-pgdump.html>.

- Dump database into an SQL-script file:

`pg_dump {{db_name}} > {{output_file.sql}}`

- Same as above, customize username:

`pg_dump -U {{username}} {{db_name}} > {{output_file.sql}}`

- Same as above, customize host and port:

`pg_dump -h {{host}} -p {{port}} {{db_name}} > {{output_file.sql}}`

- Dump a database into a custom-format archive file:

`pg_dump -Fc {{db_name}} > {{output_file.dump}}`

- Dump only database data into an SQL-script file:

`pg_dump -a {{db_name}} > {{path/to/output_file.sql}}`

- Dump only schema (data definitions) into an SQL-script file:

`pg_dump -s {{db_name}} > {{path/to/output_file.sql}}`
