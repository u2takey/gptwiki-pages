# mongoexport 
## chatgpt 
mongoexport is a command-line tool used in MongoDB for exporting data from a specified MongoDB instance to a JSON, CSV or TSV file.

The command supports a variety of parameters to customize the export process. Here are some of the most commonly used parameters:

1. --db : specifies the name of the database from which the data should be exported.

2. --collection: specifies the name of the collection from which to export data.

3. --out: specifies the output file name.

4. --fields: specifies the fields to be exported. You can use this parameter to specify the fields you want to include or exclude from the export (using a minus sign, for example: --fields -_id).

5. --type: specifies the output file format (JSON, CSV, or TSV).

6. --query: allows you to specify a query for retrieving only a subset of the data from the collection.

Overall, mongoexport is a useful command-line tool for exporting data from MongoDB to various file formats. It provides a flexible way to customize the export process and can be a great option for generating custom reports or for migrating data between different environments. 

## tldr 
 
> Produce exports of data stored in a MongoDB instance formatted as JSON or CSV.
> More information: <https://docs.mongodb.com/database-tools/mongoexport/>.

- Export a collection to `stdout`, formatted as JSON:

`mongoexport --uri={{connection_string}} --collection={{collection_name}}`

- Export the documents in the specified collection that match a query to a JSON file:

`mongoexport --db={{database_name}} --collection={{collection_name}} --query="{{query_object}}" --out={{path/to/file.json}}`

- Export documents as a JSON array instead of one object per line:

`mongoexport --collection={{collection_name}} --jsonArray`

- Export documents to a CSV file:

`mongoexport --collection={{collection_name}} --type={{csv}} --fields="{{field1,field2,...}}" --out={{path/to/file.csv}}`

- Export documents that match the query in the specified file to a CSV file, omitting the list of field names on the first line:

`mongoexport --collection={{collection_name}} --type={{csv}} --fields="{{field1,field2,...}}" --queryFile={{path/to/file}} --noHeaderLine --out={{path/to/file.csv}}`

- Export documents to `stdout`, formatted as human-readable JSON:

`mongoexport --uri={{mongodb_uri}} --collection={{collection_name}} --pretty`

- Display help:

`mongoexport --help`
