# groupadd 
## chatgpt 
The `groupadd` command is used to add a new group to the system. It is a Linux/Unix command that is used from the terminal. 

Syntax: `groupadd [options] groupname`

Here, `groupname` refers to the name of the group that you want to create. 

Some of the common options used with the `groupadd` command are: 

1. `-g`: This option is used to specify the numerical ID for the group. If this option is not used, the next available ID will be assigned automatically. 

2. `-K`: This option is used to set the default password expiration policy for the new group. 

3. `-r`: This option is used to create a system group. System groups have a GID (Group ID) in the range of 0 to 999. 

4. `-f`: This option is used to force the creation of the group even if the group already exists. 

Once you have created a new group using the `groupadd` command, you can add users to the group by using the `usermod` command. The syntax for adding a user to a group is as follows: 

`usermod -aG groupname username`

Here, `groupname` refers to the name of the group that you want to add the user to and `username` refers to the name of the user that you want to add to the group. 

Overall, the `groupadd` command is a useful command for managing user groups in a Linux/Unix system. 

## tldr 
 
> Add user groups to the system.
> See also: `groups`, `groupdel`, `groupmod`.
> More information: <https://manned.org/groupadd>.

- Create a new group:

`sudo groupadd {{group_name}}`

- Create a new system group:

`sudo groupadd --system {{group_name}}`

- Create a new group with the specific groupid:

`sudo groupadd --gid {{id}} {{group_name}}`
