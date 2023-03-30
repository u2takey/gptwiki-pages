# su 
## chatgpt 
The 'su' command is a Unix/Linux command that stands for "switch user" or "superuser", and it is used to switch to another user account or to escalate privileges to the root user account. When used without any arguments, 'su' defaults to switching to the root user account.

Syntax:
  $ su [username]

To switch to another user account, you must specify the username of the target user. Once you enter the command and press Enter, you will be prompted to enter the password for the target user account. If the password is correct, you will become logged in as that user, and any command you execute will be executed with the same privileges as that user.

To escalate privileges to the root user account, simply enter 'su' without any arguments. You will be prompted to enter the password for the root user account. If you supply the correct password, you will become the root user and be able to execute any command on the system with full administrative privileges.

Note that while logged in as the root user, you have the power to make changes that could harm your system or delete important files, so it should be used with caution. It is best to switch back to a normal user account when you are finished performing administrative tasks. 

## tldr 
 
> Switch shell to another user.
> More information: <https://manned.org/su>.

- Switch to superuser (requires the root password):

`su`

- Switch to a given user (requires the user's password):

`su {{username}}`

- Switch to a given user and simulate a full login shell:

`su - {{username}}`

- Execute a command as another user:

`su - {{username}} -c "{{command}}"`
