# mongo 
## chatgpt 
mongo is a command that is used to start the MongoDB shell. When executed, it opens an interactive shell environment where you can interact with the MongoDB server and perform various database operations. The command connects to a MongoDB instance on the local machine by default, but you can also specify the host and port of a different MongoDB instance using command-line options. 

Once you start the MongoDB shell using the mongo command, you can perform various operations such as querying, inserting, deleting or updating data in the MongoDB database, creating and dropping collections, creating and using databases, and running JavaScript commands, among other things.

The MongoDB shell is a powerful command-line tool for MongoDB that enables you to test queries or debug applications using the MongoDB database. It is often used by developers, database administrators, and others who work with MongoDB to interact with the database and perform various operations. 

## tldr 
 
> MongoDB interactive shell client.
> More information: <https://docs.mongodb.com/manual/reference/program/mongo>.

- Connect to a database:

`mongo {{database}}`

- Connect to a database running on a given host on a given port:

`mongo --host {{host}} --port {{port}} {{database}}`

- Connect to a database with a given username; user will be prompted for password:

`mongo --username {{username}} {{database}} --password`

- Evaluate a JavaScript expression on the database:

`mongo --eval '{{JSON.stringify(db.foo.findOne())}}' {{database}}`
