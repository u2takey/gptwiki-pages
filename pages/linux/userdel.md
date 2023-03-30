# userdel 
## chatgpt 
The `userdel` command is used in Linux and Unix operating systems to delete a user account. It removes the user's account and any files or directories associated with that account. 

Syntax:
```
userdel [options] username
```

Options:
- `-r`: removes the user's home directory and mail spool.
- `-f`: forces the removal of the user account, even if the user is currently logged in.
- `-Z`: removes the SELinux user mapping for the user.
- `-R`: changes the location of the user's home directory to a new location provided as the argument.

Example:
```
userdel -r john
```
This command will remove the user account `john` along with its home directory and mail spool. The `-r` option is used to remove these associated files.

Note: Only root or a user with sudo privileges can use the userdel command. It is also recommended to backup any important data associated with the user account before deleting it. 

## tldr 
 
> Remove a user account or remove a user from a group.
> See also: `users`, `useradd`, `usermod`.
> More information: <https://manned.org/userdel>.

- Remove a user:

`sudo userdel {{username}}`

- Remove a user in other root directory:

`sudo userdel --root {{path/to/other/root}} {{username}}`

- Remove a user along with the home directory and mail spool:

`sudo userdel --remove {{username}}`
