# useradd 
## chatgpt 
"useradd" is a command in Linux/Unix systems used to add a new user account. When executed, this command creates a new user account by creating an entry for the user in the system's user database. 

The syntax of the command is as follows:

useradd [options] username

Here, "options" are optional parameters that can be used for customizing the user account creation process, and "username" is the name of the new user account that you want to create.

Some of the commonly used options with the useradd command are:

-m or --create-home: This option tells the command to create a home directory for the new user

-s or --shell: This option specifies the default login shell for the new user

-g or --gid: This option specifies the default primary group for the new user

-d or --home: This option specifies the location for the new user's home directory

-c or --comment: This option allows you to add a comment or description for the new user

Once the useradd command is executed with the desired options and username, a new entry is added to the system's user database with the specified information. The newly created user account can then be accessed and managed using other Linux/Unix commands/tools. 

## tldr 
 
> Create a new user.
> See also: `users`, `userdel`, `usermod`.
> More information: <https://manned.org/useradd>.

- Create a new user:

`sudo useradd {{username}}`

- Create a new user with the specified user id:

`sudo useradd --uid {{id}} {{username}}`

- Create a new user with the specified shell:

`sudo useradd --shell {{path/to/shell}} {{username}}`

- Create a new user belonging to additional groups (mind the lack of whitespace):

`sudo useradd --groups {{group1,group2,...}} {{username}}`

- Create a new user with the default home directory:

`sudo useradd --create-home {{username}}`

- Create a new user with the home directory filled by template directory files:

`sudo useradd --skel {{path/to/template_directory}} --create-home {{username}}`

- Create a new system user without the home directory:

`sudo useradd --system {{username}}`
