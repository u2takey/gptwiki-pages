# pg_restore 
## chatgpt 
pg_restore is a command-line utility tool in PostgreSQL which is used to restore a PostgreSQL database from an archive created by the pg_dump tool. It allows users to restore specific database objects to an existing PostgreSQL database or to a new database.

The syntax for the pg_restore command is as follows:

pg_restore [option...] [archivefile]

The options for pg_restore consist of various flags and switches that allow you to customize the restore process. Some of the common options include:

- -d, --dbname=db_name: Specifies the PostgreSQL database name to restore the archive to.
- -h, --host=hostname: Specifies the hostname or IP address of the server where the database is located.
- -p, --port=port_number: Specifies the port number to use for the connection.
- -U, --username=user_name: Specifies the username to use when connecting to the database.
- -c, --clean: Drops the existing database objects before restoring the archive.
- -j, --jobs=num_jobs: Specifies the number of parallel jobs to use for restoring the archive.
- -F, --format=format: Specifies the format of the archive file (e.g., tar, directory, custom). The default is tar.

Once you have specified the desired options, you can provide the name of the archive file to restore from. The pg_restore command will then proceed to restore the database objects from the archive to the specified database.

It should be noted that pg_restore does not restore user accounts or permissions. These will need to be recreated manually after the restore process is complete. 

## tldr 
 
> Restore a PostgreSQL database from an archive file created by pg_dump.
> More information: <https://www.postgresql.org/docs/current/app-pgrestore.html>.

- Restore an archive into an existing database:

`pg_restore -d {{db_name}} {{archive_file.dump}}`

- Same as above, customize username:

`pg_restore -U {{username}} -d {{db_name}} {{archive_file.dump}}`

- Same as above, customize host and port:

`pg_restore -h {{host}} -p {{port}} -d {{db_name}} {{archive_file.dump}}`

- List database objects included in the archive:

`pg_restore --list {{archive_file.dump}}`

- Clean database objects before creating them:

`pg_restore --clean -d {{db_name}} {{archive_file.dump}}`

- Use multiple jobs to do the restoring:

`pg_restore -j {{2}} -d {{db_name}} {{archive_file.dump}}`
