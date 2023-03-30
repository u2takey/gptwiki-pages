# mycli 
## chatgpt 
mycli is a command-line client interface for interacting with MySQL/MariaDB databases. It is an alternative to the default MySQL command-line client (mysql). It is written in Python and provides a number of additional features and enhancements over the default client.

When the mycli command is executed in a terminal or command prompt, it will start the mycli client and prompt the user to enter their credentials and database information. Once authenticated, the user will be presented with a command line interface where they can execute SQL queries and interact with their database.

Some of the features of mycli include syntax highlighting, auto-completion, multi-line editing, and support for various output formats such as CSV and JSON. It also provides additional commands and shortcuts to improve efficiency while working with databases.

Overall, mycli is a helpful tool for developers, database administrators, and anyone else who needs to interact with MySQL/MariaDB databases through the command line. 

## tldr 
 
> A CLI for MySQL, MariaDB, and Percona with auto-completion and syntax highlighting.
> More information: <https://manned.org/mycli>.

- Connect to a database with the currently logged in user:

`mycli {{database_name}}`

- Connect to a database with the specified user:

`mycli -u {{user}} {{database_name}}`

- Connect to a database on the specified host with the specified user:

`mycli -u {{user}} -h {{host}} {{database_name}}`
