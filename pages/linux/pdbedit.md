# pdbedit 
## chatgpt 
The `pdbedit` command is a tool for managing the user and group accounts stored in a Samba passdb (password database) file. The passdb file is used to authenticate users and grant them access to resources on a Samba server. 

The `pdbedit` command can perform various actions on the passdb file such as creating and deleting user accounts, modifying user properties, managing user group memberships, and listing the users and their properties.

Some common options used with the `pdbedit` command are:

- `-a` or `--add`: to add a new user to the passdb file
- `-d` or `--delete`: to delete a user from the passdb file
- `-m` or `--modify`: to modify a user's attributes such as password or group membership
- `-L` or `--list`: to list all the users in the passdb file along with their properties
- `-G` or `--group`: to manage group memberships of users

Overall, the `pdbedit` command is a powerful tool for managing the authentication and access control mechanism of a Samba file server. 

## tldr 
 
> Edit the Samba user database.
> For simple user add/remove/password, you can also use `smbpasswd`.
> More information: <https://manned.org/pdbedit>.

- List all Samba users (use verbose flag to show their settings):

`sudo pdbedit --list --verbose`

- Add an existing Unix user to Samba (will prompt for password):

`sudo pdbedit --user {{username}} --create`

- Remove a Samba user:

`sudo pdbedit --user {{username}} --delete`

- Reset a Samba user's failed password counter:

`sudo pdbedit --user {{username}} --bad-password-count-reset`
