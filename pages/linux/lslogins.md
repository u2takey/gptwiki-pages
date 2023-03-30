# lslogins 
## chatgpt 
The "lslogins" command is a Linux utility that displays information about user accounts and their properties. 

When the command is executed, it will display a list of all the user accounts registered on the system, along with their various attributes such as user ID (UID), group ID (GID), home directory, shell, and other information. The command can be particularly useful for system administrators as it allows them to quickly get an overview of all the users and their settings.

Some of the common options used with lslogins are:

- -u: Displays additional information about user accounts such as UID, GID, and GECOS fields.
- -g: Displays information about user groups.
- -h: Displays only the header line of the output.
- -o: Displays output in a tab-separated format.

Overall, the "lslogins" command is a helpful tool for managing Linux user accounts and gaining insights into their properties. 

## tldr 
 
> Show information about users on a Linux system.
> More information: <https://man7.org/linux/man-pages/man1/lslogins.1.html>.

- Display users in the system:

`lslogins`

- Display users belonging to a specific group:

`lslogins --groups={{groups}}`

- Display user accounts:

`lslogins --user-accs`

- Display last logins:

`lslogins --last`

- Display system accounts:

`lslogins --system-accs`

- Display supplementary groups:

`lslogins --supp-groups`
