# mycli 
## chatgpt 
mycli is a command-line interface tool for accessing MySQL databases. 

When you enter "mycli" in the terminal or command prompt, it will open the interactive shell for mycli. 

From the mycli shell, you can connect to your MySQL database and execute SQL statements. 

Some of the features of mycli include auto-completion of SQL statements, syntax highlighting, and multiple output format options. 

To learn more about mycli and its usage, you can type "help" or "\?" in the mycli shell. 

## tldr 
 
> A command-line client for MySQL that can do auto-completion and syntax highlighting.
> More information: <https://mycli.net>.

- Connect to a local database on port 3306, using the current user's username:

`mycli {{database_name}}`

- Connect to a database (user will be prompted for a password):

`mycli -u {{username}} {{database_name}}`

- Connect to a database on another host:

`mycli -h {{database_host}} -P {{port}} -u {{username}} {{database_name}}`
