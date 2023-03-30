# gpasswd 
## chatgpt 
The `gpasswd` command is a tool used on Linux and Unix-like operating systems to manage group memberships. It is used to add and remove users from groups or to assign a new group owner.

Syntax:
```
gpasswd [options] groupname
```

Common options include:

- `-a, --add`: adds a user to a group
- `-d, --delete`: removes a user from a group
- `-r, --remove-password`: removes the group password
- `-M, --members`: lists the members of a group
- `-A, --administrators`: lists the administrators of a group
- `-R, --restrictions`: sets group ownership restrictions
- `-h, --help`: displays help information about the command

Here's an example command to add a user "alice" to the group "developers":
```
gpasswd -a alice developers
```

This command adds the user "alice" to the group "developers" by using the `-a` option to add a user to a group, followed by the group name. 

## tldr 
 
> Administer `/etc/group` and `/etc/gshadow`.
> More information: <https://manned.org/gpasswd>.

- Define group administrators:

`sudo gpasswd -A {{user1,user2}} {{group}}`

- Set the list of group members:

`sudo gpasswd -M {{user1,user2}} {{group}}`

- Create a password for the named group:

`gpasswd {{group}}`

- Add a user to the named group:

`gpasswd -a {{user}} {{group}}`

- Remove a user from the named group:

`gpasswd -d {{user}} {{group}}`
