# passwd 
## chatgpt 
The `passwd` command is a command-line utility used to change a user's password. When executed, it prompts the user to enter their current password and then enter a new password. 

If the user enters the correct current password, the system will change the password to the new one. If the user enters an incorrect password or the new password does not meet the system's password complexity requirements, the command will fail and an error message will be displayed. 

The `passwd` command can only be used by the root user or by users who have been granted permission to change passwords. It is an essential tool for maintaining the security of users' accounts and ensuring that their passwords are not easily guessed or compromised. 

## tldr 
 
> Passwd is a tool used to change a user's password.
> More information: <https://manned.org/passwd>.

- Change the password of the current user interactively:

`passwd`

- Change the password of a specific user:

`passwd {{username}}`

- Get the current status of the user:

`passwd -S`

- Make the password of the account blank (it will set the named account passwordless):

`passwd -d`
