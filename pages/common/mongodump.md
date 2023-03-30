# mongodump 
## chatgpt 
mongodump is a command-line tool for creating backups of MongoDB databases. It allows users to extract data from remote or local databases and save it in a specified directory on their computer. Here is a breakdown of the mongodump command:

- 'mongodump' is the actual command being used.
- The syntax of the command is relatively simple, and many of the parameters are optional.
- By default, mongodump will attempt to connect to a MongoDB process running on the local machine.
- The tool can also be used to connect to a remote MongoDB instance by specifying a host and port number.
- The available input parameters include options for specifying the output directory, compression, authentication, and more.
- The resulting backup files can be restored with the mongorestore command.
- When a mongodump command is run, it will generate a folder containing all of the data from the target database. This includes all of the Collections present in the database.
- These files can be used to create a new database from scratch or to restore an existing database to a previous state.
- mongodump is a valuable tool for any MongoDB administrator who wants to maintain the integrity of their data by creating regular backups. 

## tldr 
 
> Utility to export the contents of a MongoDB instance.
> More information: <https://docs.mongodb.com/database-tools/mongodump/>.

- Create a dump of all databases (this will place the files inside a directory called "dump"):

`mongodump`

- Specify an output location for the dump:

`mongodump --out {{path/to/directory}}`

- Create a dump of a given database:

`mongodump --db {{database_name}}`

- Create a dump of a given collection within a given database:

`mongodump --collection {{collection_name}} --db {{database_name}}`

- Connect to a given host running on a given port, and create a dump:

`mongodump --host {{host}} --port {{port}}`

- Create a dump of a given database with a given username; user will be prompted for password:

`mongodump --username {{username}} {{database}} --password`

- Create a dump from a specific instance; host, user, password and database will be defined in the connection string:

`mongodump --uri {{connection_string}}`
