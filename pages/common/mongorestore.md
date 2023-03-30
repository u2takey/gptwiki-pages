# mongorestore 
## chatgpt 
mongorestore is a command line tool provided by MongoDB to restore data from a binary or JSON format dump created using mongodump or any other backup tool.

To use the mongorestore command, the user must provide the following:

1. The path to the dump directory or archive file that contains the backup.

2. The host and port number of the MongoDB instance where the data will be restored.

3. The authentication details (username and password) if the MongoDB instance requires authentication.

4. Optional parameters like --db and --collection to restore specific databases or collections.

When mongorestore is executed with these parameters, it connects to the MongoDB instance and restores the data from the dump file. It creates new databases or collections if they don't exist already, and adds the data to the existing ones.

The mongorestore command can also restore index definitions, users, and roles that are backed up using mongodump. The user can use the --indexes, --users, and --roles options to restore these entities.

Overall, the mongorestore command provides an efficient way to restore data from backups in a production system or to migrate data from one MongoDB instance to another. 

## tldr 
 
> Utility to import a collection or database from a binary dump into a MongoDB instance.
> More information: <https://docs.mongodb.com/database-tools/mongorestore/>.

- Import a BSON data dump from a directory to a MongoDB database:

`mongorestore --db {{database_name}} {{path/to/directory}}`

- Import a BSON data dump from a directory to a given database in a MongoDB server host, running at a given port, with user authentication (user will be prompted for password):

`mongorestore --host {{database_host:port}} --db {{database_name}} --username {{username}} {{path/to/directory}} --password`

- Import a collection from a BSON file to a MongoDB database:

`mongorestore --db {{database_name}} {{path/to/file}}`

- Import a collection from a BSON file to a given database in a MongoDB server host, running at a given port, with user authentication (user will be prompted for password):

`mongorestore --host {{database_host:port}} --db {{database_name}} --username {{username}} {{path/to/file}} --password`
