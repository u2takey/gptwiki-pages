# setfacl 
## chatgpt 
The "setfacl" command in Linux is used to set file access control lists (ACLs) on a file or directory. ACLs allow more granular control over file permissions than traditional Unix-style permission models. 

The basic syntax of the "setfacl" command is as follows: 

```
setfacl -option(s) permissions file/directory 
```

Here's what each component of the command does: 
- "setfacl" is the name of the command 
- "-option(s)" are optional arguments that modify the behavior of the command. Some common options include: 
    - "-m": modify an existing ACL
    - "-x": remove an ACL
    - "-R": apply the ACL recursively to all files and subdirectories within a directory 
- "permissions" specify the permissions to grant or revoke. The format of the permissions varies depending on the filesystem and kernel version, but examples include: 
    - "u:user:rwx": grant the specified user read, write, and execute permissions
    - "d:u:user:rwx": grant default permissions to the specified user
- "file/directory" specifies the file or directory whose ACL will be modified 

Here are a few examples of how to use "setfacl": 

1. Grant read and write access to a user on a file: 

```
setfacl -m u:bob:rw myfile.txt
```

2. Grant read, write, and execute access to a group on a directory and all its contents: 

```
setfacl -R -m g:admins:rwx mydirectory
```

3. Remove all ACLs from a file: 

```
setfacl -b myfile.txt
``` 

## tldr 
 
> Set file access control lists (ACL).
> More information: <https://manned.org/setfacl>.

- Modify ACL of a file for user with read and write access:

`setfacl -m u:{{username}}:rw {{file}}`

- Modify default ACL of a file for all users:

`setfacl -d -m u::rw {{file}}`

- Remove ACL of a file for a user:

`setfacl -x u:{{username}} {{file}}`

- Remove all ACL entries of a file:

`setfacl -b {{file}}`
