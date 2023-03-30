# createdb 
## chatgpt 
The "createdb" command is used to create a new database in PostgreSQL. This command can be used in a command line interface or in a graphical user interface tool such as pgAdmin.

The syntax for the "createdb" command is as follows:

```
createdb [options] [dbname]
```

Where "options" specify any additional configuration settings for the new database, and "dbname" is the name of the new database that you want to create.

For example, to create a new database called "mynewdb", you would enter the following command:

```
createdb mynewdb
```

This will create a new database with default settings and the name "mynewdb".

You can also specify additional options to configure the new database. Some commonly used options include:

- "-O username": Specifies the owner of the new database.
- "-E encoding": Specifies the character encoding for the new database.
- "-T template": Specifies a template database to use as a basis for the new database.

For example, to create a new database called "mynewdb" owned by the user "myuser", with UTF-8 encoding and based on a template called "mytemplate", you would enter the following command:

```
createdb -O myuser -E UTF8 -T mytemplate mynewdb
```

This will create a new database with the specified settings and the name "mynewdb". 

## tldr 
 
> Create a PostgreSQL database.
> More information: <https://www.postgresql.org/docs/current/app-createdb.html>.

- Create a database owned by the current user:

`createdb {{database_name}}`

- Create a database owned by a specific user with a description:

`createdb --owner={{username}} {{database_name}} '{{description}}'`

- Create a database from a template:

`createdb --template={{template_name}} {{database_name}}`
