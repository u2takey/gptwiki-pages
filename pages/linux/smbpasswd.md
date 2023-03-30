# smbpasswd 
## chatgpt 
The smbpasswd command is used to create, modify or reset user accounts that can be used to access Samba shares on a Linux machine from other computers on the same network. It is a command-line tool that is similar to the passwd command used to manage user accounts on a Linux system.

The smbpasswd command can be used for the following tasks:

1. Create a new user account: To create a new user account for accessing Samba shares, you can use the smbpasswd command followed by the -a option and the username of the new user. For example, the command smbpasswd -a john will create a new Samba user account for a user named john.

2. Change the password for a user: To change the password for an existing Samba user, you can use the smbpasswd command followed by the username of the user. For example, the command smbpasswd mary will prompt you to enter a new password for the Samba user named mary.

3. Delete a user account: To delete a Samba user account, you can use the smbpasswd command followed by the -x option and the username of the user you want to delete. For example, the command smbpasswd -x bob will delete the Samba user account for a user named bob.

4. Reset the password for a user: To reset the password for an existing Samba user, you can use the smbpasswd command followed by the -r option and the username of the user. For example, the command smbpasswd -r alice will prompt you to enter a new password for the Samba user named alice.

Overall, the smbpasswd command is an essential tool for managing Samba user accounts and ensuring secure access to Samba shares on a Linux machine. 

## tldr 
 
> Add/remove a Samba user or change its password.
> Samba users must have an existing local Unix account.
> More information: <https://manned.org/smbpasswd.8>.

- Change the current user's SMB password:

`smbpasswd`

- Add a specified user to Samba and set password (user should already exist in system):

`sudo smbpasswd -a {{username}}`

- Modify an existing Samba user's password:

`sudo smbpasswd {{username}}`

- Delete a Samba user (use `pdbedit` instead if the Unix account has been deleted):

`sudo smbpasswd -x {{username}}`
