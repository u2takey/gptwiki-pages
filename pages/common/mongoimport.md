# mongoimport 
## chatgpt 
The `mongoimport` command tool is used to import data from a JSON, CSV, or TSV file into a MongoDB database. 

The syntax of the command is as follows:

```
mongoimport [options] <connection-string> <file>
```

Here, the `options` refer to the various additional parameters that can be used with the command, such as specifying the database or collection to import the data into, defining the format of the input file, providing authentication credentials, and more.

The `connection-string` parameter refers to the connection string for the MongoDB database or deployment, and typically includes the hostname, port number, and authentication details.

The `file` parameter is the path to the file that contains the data to be imported into the database. This file should be in JSON, CSV, or TSV format, depending on the format specified using the relevant options.

Some of the most commonly used options of the `mongoimport` command include:

- `-d/--db`: to specify the name of the database to import the data into
- `-c/--collection`: to specify the name of the collection within the database to import the data into
- `--type`: to specify the type of the input file, e.g. JSON, CSV, or TSV
- `--jsonArray`: to specify that the input file contains a JSON array, each element of which should be treated as a separate document to be imported
- `-u/--username` and `-p/--password`: to provide authentication credentials for the database

The `mongoimport` command can be run from the terminal or command prompt on the system where the MongoDB instance is running, or from a remote system that has access to the MongoDB deployment. Once the command completes successfully, the data from the input file will be imported into the specified database and collection in the MongoDB instance. 

## tldr 
 
> Imports content from a JSON, CSV, or TSV file into a MongoDB database.
> More information: <https://docs.mongodb.com/database-tools/mongoimport/>.

- Import a JSON file into a specific collection:

`mongoimport --file={{path/to/file.json}} --uri={{mongodb_uri}} --collection={{collection_name}}`

- Import a CSV file, using the first line of the file to determine field names:

`mongoimport --type={{csv}} --file={{path/to/file.csv}} --db={{database_name}} --collection={{collection_name}}`

- Import a JSON array, using each element as a separate document:

`mongoimport --jsonArray --file={{path/to/file.json}}`

- Import a JSON file using a specific mode and a query to match existing documents:

`mongoimport --file={{path/to/file.json}} --mode={{delete|merge|upsert}} --upsertFields="{{field1,field2,...}}"`

- Import a CSV file, reading field names from a separate CSV file and ignoring fields with empty values:

`mongoimport --type={{csv}} --file={{path/to/file.csv}} --fieldFile={{path/to/field_file.csv}} --ignoreBlanks`

- Display help:

`mongoimport --help`
