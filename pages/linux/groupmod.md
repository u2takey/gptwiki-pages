# groupmod 
## chatgpt 
The groupmod command in Linux is used to modify various attributes of a group. It is a Linux command that allows administrators to manage the user groups on their systems by modifying their settings.

Here are the parameters used with the groupmod command and their explanations:

- -g: This parameter is used to modify the GID (group ID) of the existing group.
- -n: This parameter is used to modify the name of the existing group.
- -o: This parameter is used to allow the creation of a group with a non-unique GID.
- -R: This parameter is used to specify the root directory path.
- -P: This parameter is used to specify the location of the group password file.

To modify a group using the groupmod command, you must be logged in as a root user or have superuser privileges. The general syntax for the command is as follows:

```
groupmod [options] group
```

For example, to change the name of a group from "sales" to "marketing", you would use the following command:

```
groupmod -n marketing sales
```

This would change the name of the group from "sales" to "marketing". Similarly, you can use the other parameters to modify other attributes of the group, such as its GID or password file location. 

## tldr 
 
> Modify existing user groups in the system.
> See also: `groups`, `groupadd`, `groupdel`.
> More information: <https://manned.org/groupmod>.

- Change the group name:

`sudo groupmod --new-name {{new_group}} {{group_name}}`

- Change the group id:

`sudo groupmod --gid {{new_id}} {{group_name}}`
