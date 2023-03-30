# getent 
## chatgpt 
getent is a command used in Linux and Unix-like operating systems to lookup and display database entries. It retrieves information from various backends, including files (such as /etc/passwd and /etc/group), Network Information Service (NIS) servers, and Lightweight Directory Access Protocol (LDAP) servers.

The syntax for the getent command is as follows:

getent database_name [key]

The database_name specifies the type of database to search, which can be one of the following:

- passwd: retrieves information about users
- group: retrieves information about groups
- shadow: retrieves information about passwords (if shadow passwords are enabled)
- hosts: retrieves information about network hosts (IP addresses, hostnames, etc.)
- services: retrieves information about network services (such as HTTP or SSH)
- protocols: retrieves information about network protocols (such as TCP or UDP)

The optional key argument restricts the search to a specific entry in the database.

For example, to retrieve information about a user named "john" from the passwd database, you can use the following command:

getent passwd john

This will display the user's entry in the passwd file, which includes their username, user ID, group ID, home directory, and shell.

Similarly, to retrieve information about a particular group, you can use the group database:

getent group developers

This will display the entry for the "developers" group, which includes the group name, group ID, and a list of its members. 

## tldr 
 
> Get entries from Name Service Switch libraries.
> More information: <https://manned.org/getent>.

- Get list of all groups:

`getent group`

- See the members of a group:

`getent group {{group_name}}`

- Get list of all services:

`getent services`

- Find a username by UID:

`getent passwd 1000`

- Perform a reverse DNS lookup:

`getent hosts {{host}}`
