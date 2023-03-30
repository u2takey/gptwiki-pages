# typeorm 
## chatgpt 
typeorm is a command that refers to the TypeORM library which is an Object-Relational Mapping (ORM) library that allows developers to interact with various Relational Database Management Systems (RDBMS). Developers can use this command to set up, create, and manage their database and its related entities in their project.

To execute the typeorm command, you need to have installed it globally on your machine. Once installed, you can use this command to manage your project's database schema, migrations, and data seeding, among other things.

The typeorm command includes several sub-commands that allow you to perform different tasks, such as:

- `typeorm init`: initializes a new TypeORM project with sample files and folders.
- `typeorm migration:create`: creates a new migration file that allows you to scaffold changes to your database schema.
- `typeorm migration:run`: applies all pending migrations to update your database schema.
- `typeorm entity:create`: creates a new entity file that models a database table.
- `typeorm query`: allows you to execute custom SQL queries on your database.

In summary, the typeorm command is an essential tool for developers using the TypeORM library because it allows them to interact with their Relational Database Management System (RDBMS) without writing complex SQL queries. With its user-friendly syntax and interface, developers can work efficiently with their database and related entities. 

## tldr 
 
> A JavaScript ORM that can run on Node.js, browser, Cordova, Ionic, React Native, NativeScript, and Electron platforms.
> More information: <https://typeorm.io/>.

- Generate a new initial TypeORM project structure:

`typeorm init`

- Create an empty migration file:

`typeorm migration:create --name {{migration_name}}`

- Create a migration file with the SQL statements to update the schema:

`typeorm migration:generate --name {{migration_name}}`

- Run all pending migrations:

`typeorm migration:run`

- Create a new entity file in a specific directory:

`typeorm entity:create --name {{entity}} --dir {{path/to/directory}}`

- Display the SQL statements to be executed by `typeorm schema:sync` on the default connection:

`typeorm schema:log`

- Execute a specific SQL statement on the default connection:

`typeorm query {{sql_sentence}}`

- Display help for a subcommand:

`typeorm {{subcommand}} --help`
