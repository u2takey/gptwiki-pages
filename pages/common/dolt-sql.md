# dolt sql 
## chatgpt 
The "dolt sql" command is used in Dolt, a relational database system that combines the Git version control system with SQL querying. 

When you use this command, it opens a prompt where you can enter SQL queries to interact with the data in your Dolt database. This includes querying data, creating and modifying tables, and running complex joins and calculations.

Here are some examples of SQL queries you can run with "dolt sql":
- "SELECT * FROM table_name" to view all rows and columns in a specific table
- "INSERT INTO table_name (column1, column2) VALUES ('value1', 'value2')" to add a new row to a table
- "UPDATE table_name SET column1 = 'new_value' WHERE column2 = 'some_condition'" to modify existing data in a table
- "CREATE TABLE new_table_name (column1 INT, column2 VARCHAR(255))" to create a new table with specified columns.

Overall, "dolt sql" is a powerful tool for managing and querying data in a version-controlled environment, allowing for collaborative data management and rollback capabilities. 

## tldr 
 
> Run a SQL query. Multiple SQL statements must be separated by semicolons.
> More information: <https://docs.dolthub.com/cli-reference/cli#dolt-sql>.

- Run a single query:

`dolt sql --query "{{INSERT INTO t values (1, 3);}}"`

- List all saved queries:

`dolt sql --list-saved`
