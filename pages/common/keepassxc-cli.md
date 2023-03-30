# keepassxc-cli 
## chatgpt 
The command "keepassxc-cli" is a command-line interface for the KeepassXC password manager. KeepassXC is an open-source password manager that stores your passwords and other sensitive information in an encrypted database, protected by a master password or key file. The command-line interface allows you to interact with the database from the command-line or terminal, using various commands and options.

The "keepassxc-cli" command can be used to perform various tasks related to the KeepassXC password manager, such as creating a new database, opening an existing database, adding, editing, or deleting entries, generating passwords, and more. Some of the commonly used commands and options with "keepassxc-cli" are:

- "help": The "help" command displays a list of all the available commands and their usage.
- "ls": The "ls" command lists all the entries in the currently open database.
- "get": The "get" command retrieves the value of a specific field for a given entry.
- "set": The "set" command sets the value of a specific field for a given entry.
- "add": The "add" command adds a new entry to the current database.
- "remove": The "remove" command removes an entry from the current database.
- "generate": The "generate" command generates a new random password.
- "-k/--key-file": The "-k/--key-file" option specifies the path to the key file that should be used to unlock the database.

Overall, the "keepassxc-cli" command provides a powerful and flexible way to manage your passwords and other sensitive information from the command-line, which can be particularly useful for automation and scripting tasks. 

## tldr 
 
> Command-line interface for KeepassXC.
> More information: <https://manned.org/keepassxc-cli>.

- Search entries:

`keepassxc-cli lookup {{path/to/database_file}} {{name}}`

- List the contents of a folder:

`keepassxc-cli ls {{path/to/database_file}} {{/path/to/directory}}`

- Add an entry with an auto-generated password:

`keepassxc-cli add --generate {{path/to/database_file}} {{entry_name}}`

- Delete an entry:

`keepassxc-cli rm {{path/to/database_file}} {{entry_name}}`

- Copy an entry's password to the clipboard:

`keepassxc-cli clip {{path/to/database_file}} {{entry_name}}`

- Copy a TOTP code to the clipboard:

`keepassxc-cli clip --totp {{path/to/database_file}} {{entry_name}}`

- Generate a passphrase with 7 words:

`keepassxc-cli diceware --words {{7}}`

- Generate a password with 16 printable ASCII characters:

`keepassxc-cli generate --lower --upper --numeric --special --length {{16}}`
