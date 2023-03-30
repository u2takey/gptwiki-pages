# nologin 
## chatgpt 
The "nologin" command is used to disable login shell access for an existing user account on a Linux or Unix system. When the nologin command is set for a user, they are unable to access their shell and log into the system, and they will be greeted with a message that explains they are not allowed to login.

The main purpose of using the nologin command is to create a user account that has access to specific functions, such as running a particular service or performing automated tasks, without allowing them shell access to the system. This can help improve security and prevent unauthorized access to the system.

The nologin command is often used in conjunction with the /etc/passwd file, which contains user account information, to set a user account's shell to nologin. The syntax for setting a user's shell to nologin in the /etc/passwd file is as follows:

username:x:uid:gid:gecos:/home/username:/usr/sbin/nologin

In this example, "username" is the name of the user account, "uid" is the user ID, "gid" is the group ID, "gecos" is the comment field, and "/usr/sbin/nologin" is the shell field.

Overall, the nologin command is a useful tool for system administrators who need to create user accounts with limited access to the system. By preventing shell access, the nologin command can help improve security and prevent unauthorized system access. 

## tldr 
 
> Alternative shell that prevents a user from logging in.
> More information: <https://manned.org/nologin.5>.

- Set a user's login shell to `nologin` to prevent the user from logging in:

`chsh -s {{user}} nologin`

- Customize message for users with the login shell of `nologin`:

`echo "{{declined_login_message}}" > /etc/nologin.txt`
