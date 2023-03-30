# query 
## chatgpt 
In general, a query command is used to retrieve specific data from a database or other forms of data storage. The exact syntax and functionality of the query command will depend on the specific database management system or software being used.

The basic structure of a query command usually consists of specifying the table or tables from which data is to be retrieved and using various query operators and filters to narrow down the results. For example, a simple query command might look like this:

SELECT * FROM customers WHERE state = 'CA';

In this example, the command is selecting all columns from the 'customers' table where the state column equals 'CA'.

Query commands can also be used to perform more complex tasks such as joining multiple tables, sorting and grouping data, and performing calculations on data. The specific syntax and options for these tasks will depend on the database management system in use.

Overall, the query command is an essential tool for retrieving and analyzing data stored in databases or other data storage systems. 

## tldr 
 
> Displays information about user sessions and process.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/query>.

- Display all user sessions:

`query session`

- Display the current user sessions on a remote computer:

`query session /server:{{hostname}}`

- Display logged in users:

`query user`

- Display all user sessions on a remote computer:

`query session /server:{{hostname}}`

- Display all running processes:

`query process`

- Display running processes by session or user name:

`query process {{session_name|user_name}}`
